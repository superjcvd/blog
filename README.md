# instructions

## install
install hugo on your computer
`pacman -S hugo`
clone your blog project
`git clone git@github.com:superjcvd/blog.git`

## configure
edit 'config.toml' file
```
baseURL = "https://superjcvd.github.io/blog/"
languageCode = "en-us"
title = "My new blog"
theme = "ananke"
```

## create new site
```
cd blog
hugo new site quickstart
cd quickstart

//theme
git init
git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke
echo 'theme = "ananke"' >> config.toml
```

## create and test content
```
hugo new posts/my-first-post.md
nano posts/my-first-post.md
hugo server -D
```

## generate pages
it will generate statics files into /docs
```
hugo -D
```
