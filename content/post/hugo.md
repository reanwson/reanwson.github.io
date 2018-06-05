---
title: "Hugo"
date: 2018-06-05T17:03:54+08:00
draft: true
---
macOS 10.13.4

zsh 5.3

Hugo v0.41



Installing Hugo

    $ brew install hugo

Check Hugo version

    $ hugo version

create new site

    $ hugo new site reanwson.github.io

Add theme

    $ cd reanwson.github.io/
    $ git init
    
    $ git clone https://github.com/laozhu/hugo-nuo themes/hugo-nuo

config theme

    vim config.toml
    
    baseURL = "http://example.org/"
    languageCode = "en-us"
    title = "My New Hugo Site"


create post

    hugo new post/hello-world.md

create about page

    $ hugo new about.md
    
    $ vim content/about.md

about.md

    ---
    title: "About"
    date: 2017-08-02
    layout: "about"
    menu: "main"
    weight: 50
    comments: false
    ---
    
    Write something about you here.
    
    hugo -D --theme=hugo-nuo --baseUrl="https://reanwson.github.io/"

Add git .gitignore

```vim
vim .gitignore

.DS_Store
Thumbs.db
public/
```

generate static page

```shell
$ hugo -D
```

Links

[Hugo](https://gohugo.io/)

[Hugo Nuo](https://themes.gohugo.io/hugo-nuo/)