---
layout: post
title:  "Jekyll GitHub Page 配置踩坑"
date:   2024-05-09 12:33:11 +0800
categories: jekyll
tags: jekyll 建站
---

很久没建博客了，这次使用 Jekyll 搭建了一个，还踩了一些坑。

首先是 Github Actions 的配置，Github 自动推荐的配置用的是 ruby 2.x，似乎无法支持 jekyll-archives 插件，需要用 starter-workflows 里的配置 [starter-workflows-jekyll](https://github.com/actions/starter-workflows/blob/main/pages/jekyll.yml)。


我这个 Jekyll 实例是使用 `jekyll new myblog` 命令创建的，创建后如果用 starter-workflows 的配置，Github Actions 会报

```
Your bundle only supports platforms ["x86_64-darwin-21"] but your local platform is x86_64-linux
```

需要使用命令 `bundle lock --add-platform x86_64-linux` 添加支持 linux 平台。

很多 jekyll 主题的年代都很久远，仿佛最近几年都没有新的，默认主题 minima 感觉还挺好，所以最终选定它。minima 的 github 主页写着是 3.0 实际上并没有 3.0 的稳定发布版本，因为 3.0 有一些白天黑夜模式，但尝试之后发现问题很多，比如一些 footer 不止怎么的就不见了。最终只能用回了 2.5 稳定版。


### 参考链接

- [Jekyll Quickstart](https://jekyllrb.com/docs/)
- [I am getting this error message when trying to do "cap production deploy"](https://stackoverflow.com/questions/73432608/i-am-getting-this-error-message-when-trying-to-do-cap-production-deploy)
