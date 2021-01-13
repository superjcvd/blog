# instructions

## install
pacman -S hugo
git clone git@github.com:superjcvd/blog.git
cd blog

## create new site
hugo new site quickstart
cd quickstart
git init
git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke
echo 'theme = "ananke"' >> config.toml

## create and test content
hugo new posts/my-first-post.md
hugo server -D

## generate pages
hugo -D