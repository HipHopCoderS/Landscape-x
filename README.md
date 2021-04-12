# ⭐️ landscape-x


Hexo 主题，感谢 [xiangming](https://github.com/xiangming/landscape-plus)针对原生主题进行了样式修改优化,支持hexo 3.x 和 hexo 2.x

# [**`Demo`**](https://blog.hiphopcoder.com)


## 🌈 主题特点:  
- UI 样式进行了改动
- 最近文章 最新回复
- 卜算子统计访问量
- 百度分析，百度站长,谷歌分析，谷歌站长,360分析，360站长,Bing站长
- 添加页面滚动效果
- gitalk评论
- 打赏
- 主题图片CDN

## 🌈 依赖插件:
```
"dependencies": {
    "algoliasearch": "^3.35.1",
    "hexo": "^5.0.0",
    "hexo-abbrlink": "^2.2.1",
    "hexo-addlink": "^1.0.4",
    "hexo-admin": "^2.3.0",
    "hexo-admonition": "^1.1.2",
    "hexo-algolia": "^1.3.2",
    "hexo-auto-excerpt": "^1.1.2",
    "hexo-deployer-git": "^3.0.0",
    "hexo-easy-tags-plugin": "^1.1.0",
    "hexo-generator-archive": "^1.0.0",
    "hexo-generator-category": "^1.0.0",
    "hexo-generator-feed": "^3.0.0",
    "hexo-generator-index": "^2.0.0",
    "hexo-generator-seo-friendly-sitemap": "^0.2.1",
    "hexo-generator-tag": "^1.0.0",
    "hexo-helper-qrcode": "^1.0.2",
    "hexo-plugin-gitalk": "^0.2.0",
    "hexo-renderer-ejs": "^1.0.0",
    "hexo-renderer-marked": "^4.0.0",
    "hexo-renderer-stylus": "^2.0.0",
    "hexo-server": "^2.0.0",
    "hexo-theme-landscape": "^0.0.3",
    "hexo-toc": "^1.1.0"
  }
```

## 🌈 主题使用流程：

 * 1. 克隆主题到hexo主题 `themes` 文件加下

```bash
git clone git@github.com:HipHopCoderS/Landscape-x.git  
```


- 2. 配置 _config.yml  
把主题文件下的 _config.yml  替换hexo 项目下的 _config.yml



主要修改这几个参数，其他的参数可以参考官方的文档进行设置修改

## 🌈 配置文件关键配置
### ❄️ 网站配置
```
# Site
title: HipHop_&_Coder
subtitle: 事在人为，功不唐捐！
description: 喜欢HipHop的程序猿！
keywords:  HipHop Coder Keep Real
author: 卡尔西 
language: zh-CN 
timezone: Asia/ShangHai

# permalink (文章固定链接)
url: 替换个人网址链接
permalink: :year/:abbrlink/

# 设置主题
theme: Landscape-X 

(其他配置可以参考官网根据需求进行配置)
```

### ❄️ 主题配置
#### ⚙️ 1.网页布局配置
``` yml
## Header 
(浏览器展示配置)
menu:
  home: / 
  archive: /archives
  user: /about.html

(移动端展示配置）
mobile_menu:
  home: /
  archive: /archives
  user: /about.html

rss: /atom.xml

## Content
(首页展示截取文章文案)
excerpt_link: Read More
```

#### ⚙️ 2.侧边栏展示配置
侧边栏展示控制，顺序可以随意调整
```
## Sidebar
sidebar: right
widgets:
- recent_posts
- category
# - tag
- tagcloud
- archive
#- recent_comments
- links
- friend_links
```

#### ⚙️ 3.cdn-url 主题图片设置
网站公共区域展示图片是否使用CDN，如果配置了CDN-url,就会使用cdn图片，否则就会默认使用 source/img/ 目录下的图片
`PS`: cdn-url 适用于如下网页主题图片配置
- banner_img
- footer_img
- weixin
- qq
- favicon
- Alipay
- WeChatpay

``` yml
## Img cdn path for Links
#cdn_url: https://hexo-ali.oss-cn-beijing.aliyuncs.com/
banner_img: headerNew.png
footer_img: footerNew.jpeg
```


#### ⚙️ 4.外链配置
``` yml
## Links
(个人链接跳转，顺序可以随意调整)
links:
    github-alt: 
    zhihu: 
    weixin: weixin.png
    qq: qq.png
    weibo: 
    csdn: 
    qqmusic: 
    neteasemusic: 
    envelope-o: 
    music:
    douban:
    facebook:
    linkedin:
    twitter:


# Friend_links
(添加友链)
friend_links:
    简眸: https://jianmou.github.io


# Miscellaneous
favicon: /img/favicon.ico
twitter:
google_plus:
fb_admins:
fb_app_id:

# Baidu share
baidushare: true

#是否开启打赏功能
donate: true
#打赏文案
Alipay: /img/Alipay.jpg
WeChatpay: /img/WeChatpay.jpg
donate_message: 欣赏此文？求鼓励，求支持！

```

### ⚙️ 5.插件配置
``` yml
# Deployment
## Docs: https://hexo.io/docs/one-command-deployment
# hexo-deployer-git (https://github.com/hexojs/hexo-deployer-git)
deploy:
  - type: git
    repo: 你要部署的仓库
    branch: 你要推的分支


# hexo-plugin-gitalk (https://github.com/snowdreams1006/hexo-plugin-gitalk)
(注册gitalk, 配置个人信息)
gitalk:
  clientID: ''
  clientSecret: ''
  repo: 
  owner: 
  admin: 
  distractionFreeMode: false

# hexo-algolia (https://github.com/oncletom/hexo-algolia)
(注册algolia, 配置个人信息)
algolia:
  applicationID: ''
  apiKey: ''
  adminApiKey: ''
  indexName: ''
  chunkSize: 5000

# hexo-auto-excerpt (https://github.com/ashisherc/hexo-auto-excerpt)
(首页截取文章长度控制)
excerpt_length: 500

# hexo-addlin (https://github.com/acwong00/hexo-addlink)
(每篇文章底部版权声明，可以自由修改)
addlink:
  before_text: <div class="copyright">作者：卡尔西  </br><span>本文地址：
  after_text: </span></br> 如果本文对你有帮助，欢迎微信,QQ联系,复制转载请注明作者和原文链接，谢谢!</br> 但管努力，莫问前程，事在人为，功不唐捐 ~  </div>

# hexo-easy-tags-plugin 
(https://github.com/dailyrandomphoto/hexo-easy-tags-plugin)
(创建标签大小写忽略，防止标签冗余)
easy_tags_plugin:
  enable: true
  tag_name_case: 1
  sort_ignore_case: true

# hexo-abbrlink(https://github.com/rozbo/hexo-abbrlink)
(根据算法生成文章唯一标示)
abbrlink:
  alg: crc32
  rep: hex


### 推广分析配置
(注册个人的站长账号，配置相应信息)
# Baidu Analytics ID
baidu_analytics: 
baidu_site_verification: 

# Google Webmaster tools verification setting
# See: https://www.google.com/webmasters/
# Google Analytics
google_analytics: 
google_site_verification: 

#qihu verification setting
qihu_site_verification: 

# bing verification setting
bing_site_verification: 

```

如有问题欢迎随时联系我！
Thanks!