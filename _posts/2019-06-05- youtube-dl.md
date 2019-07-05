---
layout: post
title: youtube-dl简单使用说明
tags: youtube-dl
---

youtube-dl需要ffmpeg，所以要事先安装好ffmpeg。

## 1.查看资源
youtube-dl -F 地址

`youtube-dl -F https://www.youtube.com/watch?v=aDwrMeu4k9Y`

获得资源列表，然后记住所需资源编号，如视频248，音频251。

## 2.下载资源
youtube-dl -f 资源编号 视频地址

`youtube-dl -f 248+251 https://www.youtube.com/watch?v=aDwrMeu4k9Y`

如非视频音频分离的视频，如720P，也可以只使用一个资源编号下载

`youtube-dl -f 22 https://www.youtube.com/watch?v=aDwrMeu4k9Y`

## 3.使用代理

`--proxy socks5://127.0.0.1:1080/`

`y2b --proxy socks5://127.0.0.1:1080/ -F https://www.youtube.com/watch?v=Wvdr1xloIFs`
