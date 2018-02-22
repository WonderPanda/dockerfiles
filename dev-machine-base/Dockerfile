FROM ubuntu:16.04

RUN apt update
RUN apt -y install zsh
RUN apt -y install wget
RUN apt -y install git
RUN apt -y install vim
RUN wget https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | zsh || true
RUN git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf && ~/.fzf/install
RUN echo zsh > ~/.bash_profile
RUN echo source ~/.bash_profile > ~/.bashrc
