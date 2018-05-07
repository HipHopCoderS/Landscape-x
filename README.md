# landscape-x


Hexo 主题，感谢 [xiangming](https://github.com/xiangming/landscape-plus)针对原生主题进行了样式修改优化,支持hexo 3.x 和 hexo 2.x

# [**`Demo`**](http://blog.rapcoder.com)




主题特点:  
- UI 样式进行了改动
- 最近文章 最新回复
- 卜算子统计访问量
- 百度分析，百度站长
- 谷歌分析，谷歌站长
- 360分析，360站长
- 添加页面滚动效果



## 克隆主题到hexo主题目录下
```bash
git clone git@github.com:HipHopCoderS/Landscape-x.git  
```


## 配置 _config.yml  
把主题文件下的 _config.yml  替换hexo 项目下的 _config.yml


主要修改这几个参数，其他的参数可以参考官方的文档进行设置修改

```
# Site
title: HipHop_&_Coder
subtitle: 事在人为，功不唐捐！
description: 喜欢HipHop的程序猿！
author: 卡尔西
language: zh-CN
timezone: Asia/ShangHai
```

## 博客设置

先配置下个人的CDN ,博客中的图片引用都是通过CDN地址的, 使用中只用填写cdn 上的文件名即可，例如qq,weixin 图片的引用

```
# img CDN path
cdn-url: you cdn path
```



`links 更改为自己的个人信息`

```
links:
    github-alt: hiphopcoders
    twitter:
    zhihu: HipHopCode
    weixin: weixin.png
    qq: qq.png
    weibo: http://weibo.com/p/1005051632283810/home
    douban:
    facebook:
    linkedin:
    # 个人邮件
    envelope-o: mailto:hiphopcoder@163.com
    music: http://5sing.kugou.com/fc/8637366.html
    csdn: a542551042
```

`支持gitalk  等第三方平评论`

```
# comments 
# gittalk.enable  true  or  false 
gitalk:
  enable: false 
  clientID: 
  clientSecret: 
  repo: 
  owner: 
  admin: 

disqus_shortname:  rapcoder
```

`支持Algolia第三方搜索`

```
# Algolia
algolia:
  applicationID: ''
  apiKey: ''
  adminApiKey: ''
  indexName: ''
  chunkSize: 5000
```
如有问题欢迎随时联系我！
Thanks!