#Java系列教程

本系列教程分为两个部分：基础篇和提高篇。

## 基础篇

位于guide目录，文件和目录列表如下：
* code：示例代码
* imgs：本书用到的图片，大多数图片包含dia源文件
* *.lyx：本教材各章节lyx源代码，其中的java-guide-on-c.lyx为主控文件。
* preamble.tex：Lyx的导言设置，在这里设置纸张大小、代码列表的样式等。这些也
可以在Lyx的图形用户界面设置，但是通过导言设置便于大型文档的组织。
* frontmatter.tex：前言的latex源代码
* cover.svg：封面，使用inkscape编辑而成

## 提高篇

位于advanced目录，文件和目录列表如下：
* code：示例代码
* imgs：本书用到的图片，大多数图片包含dia源文件
* *.lyx：本教材各章节lyx源代码，其中的java-advanced.lyx为主控文件。
* preamble.tex：Lyx的导言设置，在这里设置纸张大小、代码列表的样式等。这些也
可以在Lyx的图形用户界面设置，但是通过导言设置便于大型文档的组织。
* frontmatter.tex：前言的latex源代码
* cover.svg：封面，使用inkscape编辑而成

# 为什么选用Lyx编写本书？

本系列教材是写给程序员或者未来的程序员读的，程序员要求有很高的抽象思维和
逻辑思维能力，word之流只能培养乱写乱画的能力，所以，Lyx是编写计算机类图书
的首选工具:-)。

其实上手Lyx很容易，相信用过的都会爱不释手。Lyx自带的用户指南简洁实用，
关于使用Lyx的一些经验教训，您也可以参考博客：http://dz.sdut.edu.cn/blog/subaochen/category/lyxlatex/

# 如何参与

## 搭建书写环境

如果您仅仅是为了阅读，请下载本项目，到相应目录下执行./makebook.sh即可生成
相应的pdf文件。在阅读本书过程中，您遇到任何问题或者有任何建议、意见，欢迎
提交issue或者邮件联系作者。

如果您希望共同完善本教程，请继续往下读。

本教程使用lyx 2+编写，搭建书写环境的步骤是：
 * 建议安装Linux环境，作者是在Linux环境下编写本书的。
 * 安装textlive最新版和lyx 2+。
 * fork本项目，clone项目到本地。
 * 执行common中的deploy.sh脚本安装lyx的几个模块，然后启动lyx，点击“工具”->"重配置"，重启lyx
 * lyx java-guide-on-c.lyx（基础篇），或者lyx java-advanced.lyx（提高篇），
 即可开始愉快的写作:-)
 * 执行./makebook.sh可以生成本书的pdf文件（包含封面），请到上一级目录查看生成的pdf文件。
 如果只是日常编辑的话，这一步可以忽略。
 * 提交PR或者issue。

## 管理参考文献

本系列教程的参考文献使用BibTex(www.bibtex.org)，在common目录下的java.bib和
other.bib分别是Java相关的参考文献以及其他参考文献。可以手工编写BibTex文件，
也可以使用jabref(http://www.jabref.org/)管理参考文献，很方便。

在插入参考文献时，采用类似如下的格式[4,p101,人工智能的未来]，其中：

* 表示参考文献列表的第4项，这个由Latex自动产生。
* p101表示引用文献的第101页，这需要在添加文献引用的时候明确说明，
在Lyx中，需要在“文字后”的文本框填写。
* “人工智能的未来”，是所引用文献的标题，如果存在的话。

happy writting now:-)
