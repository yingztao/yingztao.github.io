---
layout: post
title: "用 Apple Music 来推荐喜欢的歌曲吧"
categories: 技术宅
---

闲来无事逛 Apple 官网，莫名看到了一个叫 MusicKit 的屌屌的东西，貌似可以在第三方 App 和网站上植入 Apple Music 内的歌曲！然后我硬着头皮看了 MusicKit 的 Keynote 演讲后，觉得还是算了不要瞎折腾了。

但是！我在角落里看到了介绍能简单的将 Apple Music 中的音乐分享到网站上的方式！真的是一键分享哦！

具体操作是打开 iTunes 中的 Apple Music，选择你想要分享的专辑或者歌曲，点击右侧的三个点选择「分享」，再选择「</> 拷贝嵌入代码」。 

复制下来的代码是这个样子的：

```
<iframe allow="autoplay *; encrypted-media *; fullscreen *" frameborder="0" height="150" style="width:100%;max-width:660px;overflow:hidden;background:transparent;" sandbox="allow-forms allow-popups allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-top-navigation-by-user-activation" src="https://embed.music.apple.com/cn/album/starman/1039796877?i=1039797280"></iframe>
```

将其直接粘贴到文章中就行啦！最终展示出来的就是这个样子👇

<iframe allow="autoplay *; encrypted-media *; fullscreen *" frameborder="0" height="150" style="width:100%;max-width:660px;overflow:hidden;background:transparent;" sandbox="allow-forms allow-popups allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-top-navigation-by-user-activation" src="https://embed.music.apple.com/cn/album/starman/1039796877?i=1039797280"></iframe>

播放界面一如既往的 Apple 风格。然而貌似未登录的话每首歌曲只能播放 30 秒的样子😂，真的只能作为歌曲推荐啊！右上角登录 Apple ID 以后就可以试听全曲了，当然仅限于订阅了 Apple Music 的用户了。