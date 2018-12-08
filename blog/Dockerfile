FROM node:9
MAINTAINER : fulln <i@fulln.me>
#创建app目录,保存我们的代码

RUN mkdir -p /opt/blog
#设置工作目录
WORKDIR /opt/blog
RUN npm install -g hexo-cli
RUN hexo init /opt/blog
RUN ln -s  /opt/blog/hexo /hexo
RUN rm -rf /opt/blog/source/_posts/hello-world.md

#复制所有文件到 工作目录。
COPY ./source /opt/blog/source
COPY ./themes /opt/blog/themes
COPY ./_config.yml /opt/blog/_config.yml
COPY ./public  /opt/blog/public 

CMD ["hexo","s"]




