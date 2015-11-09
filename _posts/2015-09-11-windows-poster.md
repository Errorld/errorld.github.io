---
layout: post
title: windows上的JEKYLL发布用bat脚本
date: 2015-11-09
categories: blog
tags: [jekyll,cmd,windows]
description:


---
newp.bat:

`subl d:\\Documents\\GitHub\\errorld.github.io\\_posts\\%date:~10,4%-%date:~7,2%-%date:~4,2%-%1.md`

pushp.bat：

    git add *
    git commit -a -m 'new post'
    git push
