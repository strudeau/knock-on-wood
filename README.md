# Knock on Wood

Blog built using:

* hugo
* Academic theme https://sourcethemes.com/academic

## Initial setup

Using git, fork https://github.com/sourcethemes/academic-kickstart#fork-destination-box to knock-on-wood

then

    git clone https://github.com/strudeau/knock-on-wood knock-on-wood
    cd knock-on-wood
    git submodule update --init --recursive


## Building

    docker run --rm -it -v "C:\Users\simon\Documents\mon blog:/src" -v "C:\Users\simon\Documents\mon blog/output:/target" klakegg/hugo:ext

## Run Server

    docker run --rm -it -v "C:\Users\simon\Documents\mon blog:/src" -v "C:\Users\simon\Documents\mon blog/output:/target" -p 1313:1313 klakegg/hugo:ext server -D

## Creating a new blog post

see `Create a blog post` in https://sourcethemes.com/academic/docs/managing-content/

    docker run --rm -it -v "C:\Users\simon\Documents\mon blog:/src" -v "C:\Users\simon\Documents\mon blog/output:/target" -p 1313:1313 klakegg/hugo:ext server -D new  --kind post post/my-article-name
