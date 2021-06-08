---
title: '【AEdebug】Media Encoder 輸出 mp4 無法播放'
date: Mon, 16 Mar 2020 10:35:54 +0000
draft: false
image: aedebug-media-encoder-mp4-xmp-empty.png
slug: aedebug-media-encoder-mp4-xmp-empty
categories:
    - AfterEffects技巧
tags:
    - AfterEffects
    - 動態設計
    - motiondesign
---

Bug
===

今天使用AE製作動畫遇到一個小問題，  
不知道為什麼輸出影片時雖然顯示完成但只有出現「xxx.mp4」「xxx.xmp」2個檔案

![](https://peckyhsieh.com/wp-content/uploads/2020/03/image-32.png)

mp4檔本身還是空的，檔案大小 0 kb  
完全不能播放

![](https://peckyhsieh.com/wp-content/uploads/2020/03/image-33.png)

研究
==

搜尋了一下英文看看有沒有類似的問題找到這一篇Adobe官方社群的提問  
[Media Encoder Exports empty MP4 and XMP file? - Adobe Support Community - 8854984](https://community.adobe.com/t5/media-encoder/media-encoder-exports-empty-mp4-and-xmp-file/td-p/8854984?page=1)

裡面就有提到需要設定「2-pass」

但我根本不知道什麼是2-pass？？  
按來按去也沒看到相關的設定@@

於是又再找一下關鍵字  
找到這篇  
[VBR一次編碼 v.s 二次編碼 | 杰客森林-單機攝影情報](https://www.jacksonlin.net/20170304-vbr-cbr/)

原來是壓縮的選項

解決問題
====

回頭找Media Encoder裡面的轉存設定  

![](https://peckyhsieh.com/wp-content/uploads/2020/03/image-34.png)

找到位元速率編碼設定為「VBR，二次」

再按render

問題就解決囉！

![](https://peckyhsieh.com/wp-content/uploads/2020/03/image-35.png)

