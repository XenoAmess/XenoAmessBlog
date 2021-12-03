---
title: 20211203清除idea中的plantuml插件缓存
date: 2021-12-03 15:29:00
tags: [ '修行' ]
my: XenoAmess

---

### 清除idea中的plantuml插件缓存

目的:

希望在升级/替换idea使用的plantuml.jar后，清理掉原来生成的图片，从而使idea重新使用plantuml.jar生成

手段:

C:\Users\xenoa\AppData\Local\JetBrains\IntelliJIdea2021.3\markdown\PlantUMLCodeGeneratingProvider

使用everything 找到命名类似这个文件夹的文件夹 删除即可
