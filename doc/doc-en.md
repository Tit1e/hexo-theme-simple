![hexo-theme-simple](https://personal-1251959693.cos.ap-chengdu.myqcloud.com/2019-03-30-%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202019-03-30%2010.46.55.png)

## Install

``` bash
hexo init Blog
cd Blog
npm install
npm install --save hexo-renderer-jade hexo-generator-feed hexo-generator-sitemap hexo-browsersync hexo-generator-archive
git clone https://github.com/Tit1e/hexo-theme-simple.git themes/simple
```

## Enable

Go to `_config.yml` and change the `theme` property to `simple` value:

```yaml
theme: simple

# Show all posts in archive page using hexo-generator-archive
archive_generator:
    per_page: 0
    yearly: false
    monthly: false
    daily: false
```

## Update

``` bash
cd themes/simple 
git pull
```

## Meta Description

If you want to set meta description information, please set `desc` property and value to each post — the better method is setting default `desc` property to your scaffolds files, just like:

```md
title: Lorem ipsum dolor
date: 2015-12-31 14:49:13
desc: Lorem ipsum dolor sit amet, consectetur.
---

Lorem ipsum dolor sit amet, consectetur adipisicing elit. Totam, non numquam saepe ex ut. Deleniti culpa inventore consectetur nam saepe!
```

result:

```html
<meta name="description" content="Lorem ipsum dolor sit amet, consectetur.">
```

If there is no `desc` property or value, hexo-theme-simple will use `page.title` and `page.author` instead of it. 

## H1~H6 Title

In fact, Hexo-theme-simple only supoort two kinds of titles: h1~h3 belongs to what i called `big title`, and h4~h6 belongs to `small title`, this means that `#` and `###` have the same styles。

Why i do this? I support that an article should be short and clean, dont let visitors spend much time to recognise the blog post structure.

Another reason is that: i don't have met a great styles to distinguish between different kinds of headers.If you have gread idea about it, please let me know.

## post excerpt

If you want to show excerpt(core content of article) to your visitors, do add HTML comment tag `<!--more-->` before else content，and finally the tag will be parsed to be a variable which represents post excerpt by Hexo:

![https://cloud.githubusercontent.com/assets/9530963/14064341/0fa3c754-f432-11e5-8ad7-5d063d4a0886.png](https://cloud.githubusercontent.com/assets/9530963/14064341/0fa3c754-f432-11e5-8ad7-5d063d4a0886.png)

## Comment Plugin

Hexo-theme-simple support two comment plugins: Disqus and Duoshuo. please set like this in your `themes/simple/_config.yml`:

```yaml
disqus: seansun
```

## Danger Block

Use html tag with special class property to render block:

```html
<div class="tip">
    预处理器很强大，但它只是编写 CSS 的辅助工具。出于对扩展和维护等方面的考虑，在大型项目中有必要使用预处理器构建 CSS；但是对于小型项目，原生的 CSS 可能是一种更好的选择。不要肆意使用预处理器！
</div>
```

![danger](https://cloud.githubusercontent.com/assets/9530963/11359678/489a510c-92b9-11e5-9256-341cef6999b6.png)

## Legends

This may lead to disappointed: i don't have spacial tool to create diagrams，but just Microsoft Powerpoint。

## Last but not Least

Focus on blog posts, not blog's styles. Have fun :) !
