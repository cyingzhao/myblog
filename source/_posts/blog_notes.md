---
title: Hexo的小技巧总结
date: 2017-10-21 14:05:31
categories: Hexo
tags: [Hexo, Next]

---

### 首页显示“阅读全文”

在首页需要显示的内容后面加上<!--more-->

``` bash
首页需要显示内容
<!--more-->
首页隐藏的内容
```
### 首页标题居中
由于next首页的文章标题不居中，看着很不舒服，需要把修改themes/next/source/css/_schemes/Mist/_posts-expanded.styl 
```
.post-title,
```
修改为
```
.post-title{
    text-align: center;
}
```

### 标签居中
修改文件themes/next/source/css/_schemes/Mist/_posts-expanded.styl
```
.post-tags {
    text-align: left; #left修改为center
    a {
      padding: 1px 5px;
      background: $whitesmoke;
      border-bottom: none;
    }
```

### 详情居中
详情 即为 “发表于 | 分类于 ” 等 ，修改文件themes/next/source/css/_variables/Mist.styl
```
$site-meta-text-align = left; #left修改为center
```

### 修改next主题
修改themes/next/_config.yml
```
# Schemes
#scheme: Muse
#scheme: Mist
scheme: Pisces
#scheme: Gemini
```

