---
layout: post
title: push-post-shell-script
date: 2015-11-09
categories: blog
tags: [shell,git,jekyll]
description: 
---

    # push post
    alias pushp=pushp
    pushp()
    {
        git add *
        git commit -m 'new post: '$title
        git push
    }
