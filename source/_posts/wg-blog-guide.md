---
uuid: 5c5da3c0-168a-11ea-8fce-adc538f4fca4
title: WG Blog Guide
s: wg-blog-guide
date: 2019-12-04 19:36:49
tags:
  - hexo
  - guide
categories:
  - Technology
coauthor: liupeixin
---
[![Build Status](https://github.com/wisdom-garden/wisdom-garden.github.io/workflows/build/badge.svg)](https://github.com/wisdom-garden/wisdom-garden.github.io/workflows/build/badge.svg)


## Prerequisites
* node
* git
* github
* nvm (optional)
* git config --global user.name "your name will be show blog"
* join team: [Wisdom Garden](https://github.com/wisdom-garden)
* add SSH key to your GitHub account [help](https://help.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh)


## <a id="user-content-setup" href="#setup">Setup</a>
- `git clone -b hexo-source --recursive git@github.com:wisdom-garden/wisdom-garden.github.io.git wg-blog`
- `cd wg-blog`
- **Never checkout master**
- `git config push.default current`
- `git config --local alias.pr 'pull -r origin hexo-source'`
- `nvm use` (optional)
- `yarn global add hexo-cli` or `npm install -g hexo-cli`
- `yarn install` or `npm install`
<!-- more -->

## Write
- `Usage: hexo new [layout] <title>`
- `hexo new "title"`
- use any tool edit `~/xxxxxx/wg-blog/source/_posts/title.md`

## Preview
- `hexo serve`

## Publish
- `git pr` or ~~`git pull origin hexo-source -r`~~ only pull current branch
- `git commit`
- `git push`

## Update Article
- edit `~/xxxxxx/wg-blog/source/_posts/title.md`
- update ./source/_posts/\[title-folder\] assets
- `git commit`
- `git push`

## Delete Article
- find article in ./source/_posts/
- delete article name .md and folder
- `git commit`
- `git push`

## picture host
- recommend qiniu or sina
- manually upload get assets url use in article
- TODO: picture host tools will come in the future

## IDE Recommend
- VS Code
- Sublime Text
- Typora

## More Information
- `hexo new --help`
- `hexo --help`
- [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

## Site
- Domain: [https://blog.wisdomgarden.com](https://blog.wisdomgarden.com)

  Overseas --> [Github](https://wisdom-garden.github.io/)
  Domestic --> [Coding](http://lwkd88.coding-pages.com/)


## e.g.
- `hexo new "你好" -s hello`

url:  /2019/12/04/hello/

- `hexo new "中文"`

url: /2019/12/04/%25E4%25B8%25AD%25E6%2596%2587/
