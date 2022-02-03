<h1 align="center">Claudia</h1>
<p align="center"> 
  Concisely designed & easy to config, match device dark mode, 90+ Lighthouse scoring
</p>

<p align="center">
  <img  alt="Hexo version" src="https://img.shields.io/badge/hexo%20version-%3E%3D%206-brightgreen">
  <img  alt="GitHub license" src="https://img.shields.io/badge/LICENSE-MIT-blue">
</p>

<p align="center">
  <a href="https://haojen.github.io/Claudia-theme-blog/" rel="nofollow">Demo</a>
</p>

<p align="center">
  <span>English | </span> 
  <a href="README-CN.md" rel="nofollow">简体中文</a>
</p>

![cover](./screenshot/claudia-cover-v2.png)

## Changelog
[Recent update 02.03.2022](CHANGELOG.md)

## How to Use

### Install depend

Install to Hexo blog root directory, **Not theme directory**
```bash
npm install hexo-renderer-pug 
npm install hexo-renderer-dartsass
npm install hexo-generator-search

# if you need RSS, you must be install this plugin
npm install hexo-generator-feed
```

### User's profile

Configure the file `_config.hexo-theme-Claudia.yml` under the blog root directory

```yaml
user:
  name: 
  avatar: /images/avatar.jpg
  location:
  description:
  footnotes:

# config you SNS
social:
  zhihu:
  twitter:
  facebook:
  linkedin:
  instagram:
  github: 

```

### Upper-right navigation bar menu config

```yaml
 # main menu navigation
 menu:
   Home: /
   About: /about
   Archives: /archives
```

### Sidebar widget config
```yaml
widgets:
  - tag
  - archive
  - category
  - recent_posts
```

### Comments

#### 1. Utteranc
Documents: https://utteranc.es/

Project repo: https://github.com/utterance/utterances

```yaml
comment_utteranc:
  enable: true
  repo: Haojen/myBlogRepo # Change to your blog repo
```

#### 2. Valine
Documents： https://valine.js.org/quickstart.html

```yaml
comment_valine:
  enable: true
  appId:
  appKey:
```

### Appearance
```yaml
# 1.light 
# 2.dark
# 3.auto (default, match device appearance setting)
appearance: auto
```

### Code highlighting

1. **Disable** the default hexo highlight configuration.

```yaml
highlight:
  enable: false
```

## Analytics
Google Analytics and Baidu Analytics simple config:
```yaml
#Baidu Analytics**
ba_track_id: 

#Google Analytics
ga_track_id: 
ga_domain:
```

## Pages

### Create Post

scaffolds:

```yaml
---
title: {{ title }}
date: {{ date }}
tags:
categories:
cover: https://cover.png # if not, use the first image of the post.
---
```



### Create About Page

Create a new folder `about` under the source of hexo, and then, create a `index.md` file and copy the following content into it.

```yaml
---
title: about
date: 2018-11-09 14:50:00
updated: 2022-02-03 13:05:00
layout: about
cover: 'https://cover.jpg'
---
```



### My demo blog config

> this is original theme Demo

https://github.com/Haojen/Claudia-theme-blog

