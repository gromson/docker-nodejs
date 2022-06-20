FROM debian:latest

RUN apt-get update && \
    apt-get install curl git vim gnupg -y && \
    touch ~/.vimrc && \
    echo "set t_Co=256" > ~/.vimrc && \
    echo "syntax on" >> ~/.vimrc && \
    echo "colorscheme minimalist" >> ~/.vimrc && \
    echo "set number" >> ~/.vimrc && \
    mkdir -p ~/.vim/colors && \
    curl -o ~/.vim/colors/minimalist.vim https://raw.githubusercontent.com/dikiaap/minimalist/master/colors/minimalist.vim && \
    curl -fsSL https://deb.nodesource.com/setup_current.x | bash - && \
    apt-get install -y nodejs && \
    apt-get install -y build-essential

