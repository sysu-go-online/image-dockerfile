FROM ubuntu

RUN apt update && apt install -y g++ gdb git zsh

RUN useradd -ms /bin/zsh ubuntu
USER ubuntu

RUN git clone https://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh \
    && cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc
    
CMD /bin/zsh


ENV LANG=C.UTF-8
