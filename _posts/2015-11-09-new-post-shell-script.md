---
layout: post
title: new-post-shell-script
date: 2015-11-09
categories: blog
tags: [shell,jekyll,blog]
description: a little piece of code for jekyll post
---
    alias newp=newp
    newp()
    {
        title=$1
        pdate=`date +%Y-%m-%d`
        pname=~/errorld.github.io/_posts/$pdate-$title.md
        echo $pname
        touch $pname
        ###
        echo '---'>>$pname
        echo 'layout: post'>>$pname
        echo 'title: '$title>>$pname
        echo 'date: '$pdate>>$pname
        echo 'categories: blog'>>$pname
        echo 'tags: [,]'>>$pname
        echo 'description: '>>$pname
        echo '---'>>$pname
        ###
        vim $pname
    }

Add to .bashrc/.zshrc  

`$newp title`  
will create and open a regular md.
