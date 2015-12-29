##有了 tldr，妈妈再也不用担心我记不住命令了--Too long, Don't read --tldr

http://www.codingstyle.cn/topics/26?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io

Terminal · hkliya · 于 5 天前发布 · 最后由 fighterleslie 于 5 小时前回复 · 7795 次阅读
1
引言

有一次我在培训时说「程序员要善于使用 Terminal 以提高开发效率」，一位程序员反驳道：「这是 21 世纪，我们为什么要用落后的命令行，而不是先进的 GUI？」



是的，在一些人眼里，这个黑黑的终端窗口确实代表着落后，或者装B。
而在另一些人手里，它却是一个高效的工具。

其实很多人觉得 Terminal 难用，他们认为：

命令很多，难记
敲命令很麻烦
界面黑黑的，难看
...
我认为这些印象可能都来自于「未经任何武装」的 Terminal，实际上始终有一部分人是 Terminal 的忠实用户，他们也在推动着 Terminal 与时俱进。
所以，接下来我准备分享一系列使用 Terminal 的技巧。

目录

别再用 CD 切换目录了
「What the fuck」妈妈再也不用担心我敲错命令了

正文

使用 Terminal 最难的就是要叫住众多的 Linux 命令了，比如：ssh，curl，grep等，经常会记不住参数的顺序。

今天要介绍的工具叫：tldr。
在很多地方都会看到：「tl;dr」或「TL;DR」。
它的意思是「Too long, Don't read」，翻译成中文就是：「太长不读」。

我们可以使用man或者--help来查看特定命令的用法，但读起来效率很低。

 