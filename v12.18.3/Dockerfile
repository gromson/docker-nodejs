FROM debian:latest

RUN apt-get update && \
    apt-get install wget curl git vim gnupg -y && \
    touch ~/.vimrc && \
    echo "set t_Co=256" > ~/.vimrc && \
    echo "syntax on" >> ~/.vimrc && \
    echo "colorscheme minimalist" >> ~/.vimrc && \
    echo "set number" >> ~/.vimrc && \
    mkdir -p ~/.vim/colors && \
    wget https://raw.githubusercontent.com/dikiaap/minimalist/master/colors/minimalist.vim -O ~/.vim/colors/minimalist.vim && \
    curl -sL https://deb.nodesource.com/setup_lts.x | bash - && \
    apt-get install -y nodejs && \
    apt-get install -y build-essential

