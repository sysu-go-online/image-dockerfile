FROM python:2

RUN apt update && apt install -y g++ gdb git zsh
RUN wget https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | zsh || true
RUN useradd -ms /bin/zsh ubuntu

USER ubuntu

ENV LANG=C.UTF-8