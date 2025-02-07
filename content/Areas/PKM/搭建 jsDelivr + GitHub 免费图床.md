---
title: "jsDelivr和Github配合才是最佳免费CDN，五分钟学会使用，附搭建免费图床教程_jsdelivr怎么用-CSDN博客"
source: "https://blog.csdn.net/weixin_44786530/article/details/129851540"
author:
published:
created: 2025-02-03
description: "文章浏览阅读2.1k次，点赞3次，收藏10次。jsDelivr是一个提供数千种Javascript、CSS等超过1650多种 Libraries 加速的免费CDN服务，支持给Github、WordPress、NPM免费提供CDN加速。而且国内也有 CDN 节点，速度非常快。Github目前最好用的免费开源项目托管站点，众多开源项目都托管在Github，目前Github已被微软收购了。虽然这种免费CDN折腾起来有点麻烦，不过毕竟免费，还可以作为图床用能节省你的主机流量，加上jsDelivr 和 Github 都是大厂还是比较放心的。_jsdelivr怎么用"
tags:
  - "clippings"
---
![](https://i-blog.csdnimg.cn/blog_migrate/584eb18de0b7cba6853c9d7c23603761.png)
### jsDelivr介绍

jsDelivr是一个提供数千种Javascript、CSS等超过1650多种 Libraries 加速的免费CDN服务，支持给Github、WordPress、NPM免费提供[CDN加速](https://so.csdn.net/so/search?q=CDN%E5%8A%A0%E9%80%9F&spm=1001.2101.3001.7020)。而且国内也有 CDN 节点，速度非常快。

![](https://i-blog.csdnimg.cn/blog_migrate/45f44012fa5d2298d4f2d1fd2426e0c5.png)

**jsDelivr官方：**https://www.jsdelivr.com/

### Github介绍

Github目前最好用的免费开源项目托管站点，众多开源项目都托管在Github，目前Github已被微软收购了。

**Github官方：**https://github.com/

### 利用 jsDelivr + Github 给你的github上的文件免费加速

1.注册 Github  账号

2.新建Github仓库，Repository name：输入仓库名称，然后点击「Create repository」开始创建。

![](https://i-blog.csdnimg.cn/blog_migrate/e9ca0292252465b0c4204645706c02b6.png)

3.点击「Upload files」上传你要CDN的文件，如CSS、JS、图片等……

![](https://i-blog.csdnimg.cn/blog_migrate/be8e384f4f3da181c1170c48bec519d9.png)

4.发布仓库，点击「release」发布，输入自定义发布版本号。

![](https://i-blog.csdnimg.cn/blog_migrate/4a552489663fa0e491cea4efd7c0b3b5.png)

5.使用 jsDelivr 来引用资源

https://cdn.jsdelivr.net/gh/你的用户名/你的仓库名@发布的版本号/文件路径

例如：https://cdn.jsdelivr.net/gh/woshileifeng1/wordpresscdn@1.0/aplayer.min.js

如果不需要版本号区分，也可以直接：

https://cdn.jsdelivr.net/gh/woshileifeng1/wordpresscdn/aplayer.min.js

6.接下来把CDN好的CSS和JS等文件地址，都替换到你主题里面去。

7.可以在你主题的头部文件加入 <link rel=’dns-prefetch’ href=’//cdn.jsdelivr.net’ /> 预读DNS，加快解析

### GitHub+jsDelivr+PicGo搭建免费图床

1.新建立一个github仓库，专门存放上传的图片。

2.生成Access token

![](https://i-blog.csdnimg.cn/blog_migrate/baac9cc3a7f577a6e34f426852176dab.png)

![](https://i-blog.csdnimg.cn/blog_migrate/8b9deb4a132aa51fe7633d9763a90c18.png)

3.下载PicGo软件：https://github.com/Molunerfinn/picgo/releases

4.填入刚才在Github创建的信息，指定存储文件夹的路径，PicGo上传文件的时候，将自动在github仓库中创建此文件夹。

自定义域名：https://cdn.jsdelivr.net/gh/用户名/图床仓库名

![](https://i-blog.csdnimg.cn/blog_migrate/995e5c17aebf2ca59f285a8bd66bab42.png)

5.可以开始上传图片啦，在上传图片之后自动会将图片链接复制到你的剪贴板里。

![](https://i-blog.csdnimg.cn/blog_migrate/d6c42e6875097a856ca8b65a3d495d64.png)

### 总结

虽然这种免费CDN折腾起来有点麻烦，不过毕竟免费，还可以作为图床用能节省你的主机流量，加上jsDelivr 和 Github 都是大厂还是比较放心的