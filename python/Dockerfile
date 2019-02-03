FROM python:2

RUN apt update && apt install -y git

RUN echo "root:root" | chpasswd

CMD /bin/bash

ENV LANG=C.UTF-8
