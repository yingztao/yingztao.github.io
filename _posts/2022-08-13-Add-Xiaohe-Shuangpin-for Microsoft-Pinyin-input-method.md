---
layout: post
title: "为微软拼音输入法增加小鹤双拼"
categories: 技术宅
---

微软拼音输入法自带的双拼键位中，并没有预设小鹤双拼方案。如果我们要使用小鹤双拼的话，得自己预设一套对应的键位方案。

刚刚开始使用的时候，我是自己对照着键位表一个按键一个按键进行配置的，费时费力。现在知道了可以通过增添注册表项的方式一件添加小鹤双拼键位。

新建一个文本文档，将下方注册表内容全部复制进去，另存为后缀名师是 ”.reg“ 的注册表编辑文件。双击使用即可，即开即用。

```
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\Software\Microsoft\InputMethod\Settings\CHS]
"Enable Cloud Candidate"=dword:00000000
"Enable Dynamic Candidate Ranking"=dword:00000001
"EnableExtraDomainType"=dword:00000001
"Enable self-learning"=dword:00000001
"EnableSmartSelfLearning"=dword:00000001
"EnableLiveSticker"=dword:00000000
"Enable EUDP"=dword:00000001
"Enable Double Pinyin"=dword:00000001
"UserDefinedDoublePinyinScheme0"="小鹤双拼*2*^*iuvdjhcwfg^xmlnpbksqszxkrltvyovt"
"DoublePinyinScheme"=dword:0000000a
```

好吧实际上这东西网上教程一大堆，我只是做个自我归档而已省的要用的时候再去找……