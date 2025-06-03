---
title: chrome拒绝对自建证书以及错误证书的https网站进行任何缓存
date: 2025-02-10 23:00:00
tags: [ '修行' ]
my: XenoAmess

---

如标题所示, chrome拒绝对自建证书以及错误证书的https网站进行任何缓存

而且这是新版本新增的行为, 之前的版本是可以缓存的. 真是太好了呢, 新版本真的加了很棒的新特性呢!

所以如果你也是内网自建证书的使用者(例如企业内部网站), 你会发现你的网站的静态资源每次都会重新请求, 而不是从缓存中读取, 哪怕你的缓存策略检查了一天都怎么看都是正确的.

所以etag失效? 去骂谷歌.

cache-control失效? 去骂谷歌.

唉我的宝贵的一天浪费在了什么垃圾玩意儿上啊

### 参考资料
- [如果使用 HTTPS，浏览器不会缓存文件，即使 Web 服务器通过响应标头允许缓存](https://issues.chromium.org/issues/40140471)
- [需要测试缓存是否因证书错误而被禁用](https://issues.chromium.org/issues/40666473)
- [修改chromium代码重新编译可以解决但是这也太...](https://groups.google.com/a/chromium.org/g/chromium-dev/c/-xMWQzod7bA/m/a1vXoJav7uYJ?pli=1)
