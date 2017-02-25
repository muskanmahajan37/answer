如何真正地参与开源项目
===

对于我而言，我会参与的开源项目，一般都是**我正在使用的项目**——这是一个很重要的大前提。**只有你每天都在用，你才会知道哪里有问题，知道哪里需要改进**。

一、完善文档

**用这个开源项目，就是最好的入门**。基于这一个前提，我们再来看看，在这个项目里的新手能做点什么？先给大家看一下，我最早的几次 Pull Request。这些都是我在用这个项目的过程中，发现的问题：

1. 更新 README

![Django UUSLUG](django-uuslug.png)

这个项目也是醉了，连个安装方式都没有。

![Flask MongoDB README](../images/flask-mongodb.png)

这个是我在阅读官方文档的时候，发现怎么操作都不对。我才意识到这个文档是有问题的，顺手给了个 Pull Reqeust。这种问题很容易在 README 里找到错误。**修复的成本比较低，而且算是比较严重的错误**。

2. 代码中打错字了

![PageSpeed Issue](../images/page-speed-issues.png)

给 PageSpeed 的这次 Pull Request 是因为**代码中的一句错误提示的路径不对**。这虽然算是一个很小的语法错误，但是对于大部分人来说都是一脸懵逼。

![Sequelize Typos](../images/sequelize-typos.png)

像这种也是相似的。如果是文档错误，一般开发人员会二会不说就直接 merge 了。

3. 除此，还有一种方式是：更新依赖版本

![Update Package Version](../images/update-package-issue.png)

不过，这一招是从别人身上学的，哈哈哈。

二、提 Issue

上述的完善文档的方式，最适合于刷提交，然后就是提和处理 Issue 了。有用的 Issue 本身是在**鼓励作者，你的项目有人用呢**。如这是以前我在使用 Mezzanine 库的时候，发现在某个情况下响应特别慢：

![Mezzanine Issue](../images/mezzanine-bug.png)

然后我就去愉快地提了一个 Issue 来问作者——当时还在上学，没啥经验，不知道怎么解决。后来，发现我用的 Python 版本是 2.6，在 Python 2.7 下就没有这个问题了。相似的东西还有很多，这个时候一般来说，**是要把各种环境、条件都罗列清楚**。

当你关注一个项目很久的时候，你就可以帮作者回复 Issue 来提高好感度。这一点上，我就做得不好了，没有 watch 什么项目。不过，要是看到的时候，都会回答一下的。

三、深入代码去发现问题

1. 没有使用到的变量、方法

![多余的库](../images/remove-unused-libs.png)

这个是我在阅读代码的时候，发现的问题。在这个 seneca 项目里，明明有这么多过去使用到的，但是已经不再用的库了，于是我就给了个 Pull Request。

2. 添加一些功能支持：比如中文

![Add Language Support](../images/add-language-support.png)

对于一些插件来说，它们都只有英语，而没有中文翻译——毕竟中文对于外国人蛮难的。这个时候，就可以添加一些中文翻译。又或者是相似的修复一些中文的语法问题：

![Fix Chinese Issue](../images/auto-save-zh-issue.png)

3. 深入到项目来实现功能

大部分的开源项目都会有 Roadmap 和 Issues 列表，按上面的内容去试图实现功能就可以了。

blabla，我没啥实战经验——主要是平时自己想玩的东西比较多。




