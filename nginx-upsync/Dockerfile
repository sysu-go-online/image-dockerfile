FROM ubuntu
RUN apt update && apt install -y wget zip build-essential

RUN wget 'http://nginx.org/download/nginx-1.8.0.tar.gz' && tar -xzvf nginx-1.8.0.tar.gz
RUN wget https://codeload.github.com/weibocom/nginx-upsync-module/zip/master
RUN unzip nginx-upsync-module-master.zip
RUN rm *.tar.gz

WORKDIR /nginx-1.8.0/
RUN ./configure --add-module=/nginx-upsync-module-master && make && make install

RUN rm -rf *
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]