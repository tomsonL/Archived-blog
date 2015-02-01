---
layout: post
title:  "Jekyll入门"
date:   2015-02-01 08:04:53
categories: tecs jekyll
---

###1. 快速上手


	~ $ gem install jekyll
	~ $ jekyll new myblog
	~ $ cd myblog
	~ $ jekyll serve --detach #后台运行服务

* *访问localhost:4000就可以看到Jekyll的welcome网站了*


###2. 目录结构
	.
	├── _config.yml
	├── _drafts
	|   ├── begin-with-the-crazy-ideas.textile
	|   └── on-simplicity-in-technology.markdown
	├── _includes
	|   ├── footer.html
	|   └── header.html
	├── _layouts
	|   ├── default.html
	|   └── post.html
	├── _posts
	|   ├── 2007-10-29-why-every-programmer-should-play-nethack.textile
	|   └── 2009-04-26-barcamp-boston-4-roundup.textile
	├── _data
	|   └── members.yml
	├── _site
	└── index.html


* *_site 文件夹保存由Jekyll生成的静态站点*
* *_posts文件夹保存要发表的文章，文件名要符合下面的格式：YYYY-MM-DD-name-of-post.ext，例如2015-01-31-hello-Jekyll.markdown*


###3. 基本使用流程

1. 在_posts文件夹中创建符合命名规范的文件
2. 添加文件头：

		---
		layout: post
		title:  "Jekyll入门"
		date:   2015-02-01 08:04:53
		categories: jekyll update
		---

3. 生成站点

		$ cd /to/your/blog/root/path
		$ jekyll serve

4. localhost:4000，本地预览
5. push到github
6. 不断修改样式到你满意

###4. 更多
*详情参考[官网](http://jekyllrb.com)*
