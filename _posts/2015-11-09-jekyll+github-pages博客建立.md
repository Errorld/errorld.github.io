---
layout: post
title: github+jekyll快速搭建静态博客
date: 2015-11-09
categories: blog
tags: [github,jekyll,blog]
description: 快速简洁


---
##1. 克隆一个样本

不想从头设置就去别人的 JEKYLL-BLOG FORK一份
比如我的[github.com/errorld/errorld.github.io](http://github.com/errorld/errorld.github.io)
把名字改为user.github.io
然后克隆到本地
`$ git clone git@github.com:user/user.github.io.git

##3. 修改与发布

###1. 修改
如果不想折腾的，直接修改_config.yml里的相关内容为自己的信息就好了
要改模板也很简单，会点JINJIA就可以

###2. 发布

1. 新建
在_post下新建yyyy-mm-dd-title.md
2. 编辑
进行编辑，开头加上
```
---
layout: post
title: title
date: yyyy-mm-dd
categories: blog
tags: [tag1,tag2]
description: description

---
content
```
3. 提交
`$ git add *`
`$ git commit -m 'describe'`
`$ git push`

##3. 本地安装测试环境
###1. ruby+gem

1. RVM
`$ curl -L https://get.rvm.io | bash -s stable$ curl -L https://get.rvm.io | bash -s stable`
`$ source ~/.rvm/scripts/rvm`  
2. ruby
`$ rvm install 2.1.2`
3. nodejs
`$ sudo apt-get install nodejs`
4. 换源
`$ gem sources --add https://ruby.taobao.org/ --remove https://rubygems.org/`
5. bundle
`gem install bundle`

###2. jekyll
`$ gem install git-pages`

## Plus
如果模板不需要更改，以后只需要执行步骤2就能发布新博文。


