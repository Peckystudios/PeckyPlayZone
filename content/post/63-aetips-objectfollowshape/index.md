---

title: 【AE小技巧】如何讓物體跟著繪製的shape路徑曲線移動？
categories:
    - AfterEffects技巧
    
date: 2023-11-14 00:00:00
Description: 如果你今天有設計一條道路，你想把車子沿著這個道路移動前進，要怎麼做呢？
image: 如何讓物體跟著繪製的shape路徑曲線移動.png
slug: aetips-objectfollowshape
draft: false
tags:
    - 動態設計
    - AE
    - After Effects
    - 技巧



---


如果你今天有設計一條道路，你想把車子沿著這個道路移動前進，要怎麼做呢？

![](/F25DDABB-5C27-47EA-8511-2827DB659062.png)

AE 裡面有一個神奇的小功能可以快速的讓物體跟著我們繪製的路徑移動哦～

先讓我們看一下我們的圖層： 

![](/3F771B63-0C9B-4D39-BA04-543FCDC012FF.png)

我們現在的目標是：讓車這個圖層跟著路中線這個路徑移動。

我們先選取在「路中線」這個圖層的path屬性：

![](/4635DDEF-8A6C-4A28-BAC0-253E193E54B8.png)

這一個步驟的目的是要取得這個路徑的資訊。

下一步我們使用快捷鍵 Ctrl(Command)+C 把這個路徑的資訊複製起來。

來到「車」這個圖層，使用快捷鍵 P 將position 這個屬性叫出來：

![](/4B58ED62-85C2-4CC9-9F36-160915C25973.png)

「選擇」position這個屬性（這部很重要哦～）：

![](/2FEAB7CB-C8AE-4195-9447-5FF42E317F41.png)

使用 Ctrl(Command)+V 貼上，你會發現車車的 position 屬性多了一些 key：

![](/BBD26858-86D0-46D4-8C4E-6A30DE2FC705.png)

有些位置跑掉沒關係，在 key 全部選取的時候可以進行調整，把他調到適當的位置：

![](/9817BD0B-91EE-4EDD-970F-61DE69649AE5.png)

播放看看就會發現車車跟著路徑移動囉～

![](/project%20folder%201.gif)

接下來就可以幫他 key 上旋轉的動畫，就變成一個車車在移動的動畫啦～

![](/project%20folder%202.gif)

---

另外補充一個可能會遇到的問題，如果你遇到路徑的方向跟你要的不一樣，會遇到這個問題通常是因為你的路徑是在 illustrator 裡面繪製的，這個的話可以回到 illustrator 來修正哦～

先選取要修正的路徑：

![](/A76DAA74-1F1E-4DF8-9FBF-8ABAD5D042B7.png)

在選單的 物件 > 路徑 > 反轉路徑方向，點擊之後就會反轉了哦～

![](/AD76BE0E-02E6-47B9-BA10-4CE30958BF7F.png)

之後再重新把路徑放到 AE 裡就可以了👍🏻️

試試看吧！