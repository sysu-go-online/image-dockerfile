FROM ubuntu

RUN apt update && apt install -y g++ gdb git

RUN echo "root:root" | chpasswd
    
CMD /bin/bash

ENV LANG=C.UTF-8
