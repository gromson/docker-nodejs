FROM debian:latest

RUN apt-get update && \
    apt-get install wget git vim gnupg -y && \
    touch ~/.vimrc && \
    echo "set t_Co=256" > ~/.vimrc && \
    echo "syntax on" >> ~/.vimrc && \
    echo "colorscheme minimalist" >> ~/.vimrc && \
    echo "set number" >> ~/.vimrc && \
    mkdir -p ~/.vim/colors && \
    wget https://raw.githubusercontent.com/dikiaap/minimalist/master/colors/minimalist.vim -O ~/.vim/colors/minimalist.vim && \
    wget https://deb.nodesource.com/setup_10.x && \
    chmod +x setup_10.x && \
    ./setup_10.x && \
    apt-get install -y nodejs && \
    apt-get install -y build-essential

