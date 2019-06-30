# Table of Contents

* [1  为什么要用ipic](#1--为什么要用ipic)
* [2  ipic解决方案](#2--ipic解决方案)
  * [2.1 下载ipic（仅限mac）](#21-下载ipic（仅限mac）)
  * [2.2 偏好设置](#22-偏好设置)
  * [2.3 iPic Mover](#23-ipic-mover)
* [3  参考资料](#3--参考资料)
* [4  iPic Mover设置上传后删除本地图片](#4--ipic-mover设置上传后删除本地图片)
* [5  安装Pandoc](#5--安装pandoc)
  * [5.1 为什么要用Pandoc](#51-为什么要用pandoc)
  * [5.2 macOS](#52-macos)
* [6  github不显示toc（目录内容）](#6--github不显示toc（目录内容）)
  * [6.1 解决方案](#61-解决方案)



# 1  为什么要用ipic

在本地Typora插入图片的时候能正常显示，但是将编写的文档上传到GitHub上时，不显示了。是因为插入的时候，使用的本地链接路径，生成html文件的时候，img也是该路径，但是我们在本地存储的图片，在网站上是没有能力访问的。如下

![](http://ww2.sinaimg.cn/large/006tNc79ly1g4ixv99g4hj30kb0g1myo.jpg)

# 2  ipic解决方案

## 2.1 下载ipic（仅限mac）

在mac app store中下载，可免费使用所有功能。如需使用其他图床，订阅 iPic 高级版即可。暂不支持 Windows.

## 2.2 偏好设置

你可以在Typora的**偏好设置**中，选择**编辑器**中**图片插入**的**复制图片到当前文件夹**。最后☑️对本地位置图片应用上述规则。然后通过ipic mover统一将所有图片批量生成，生成后删除本地图片。

![image-20190630102612784](http://ww2.sinaimg.cn/large/006tNc79ly1g4iz2wtlfwj30e40e10vf.jpg)

## 2.3 iPic Mover

[iPic Mover](https://itunes.apple.com/cn/app/id1183822957?ls=1&mt=12) 可以一键将已有 Markdown 文件中所有图片迁移至新图床。批量上传图片、图床搬家，从未如此简单。

![](https://ps-hz.toolinbox.net/006y8lVagw1fajaszqardg30ia0bc4cp.gif)

这也需要App store中下载，使用之后，之前github不能显示的图片就可以显示了

![image-20190630100551123](http://ww4.sinaimg.cn/large/006tNc79ly1g4iyw35920j30pe0hiamz.jpg)

# 3  参考资料

1. [iPic - Markdown 图床、文件上传工具](https://toolinbox.net/iPic/ )

2. [Typora极简教程](https://www.jianshu.com/p/a6a6a22e9393)
3. [Github Flavored Markdown语法介绍](https://github.com/guodongxiaren/README)

# 4  iPic Mover设置上传后删除本地图片

在操作2.3时，可以将上传后删除本地图片的设置一起勾选，这里单独拿出来，是为了进行说明

![image-20190630101413952](http://ww1.sinaimg.cn/large/006tNc79ly1g4iytyj3j1j30jy0dwaaj.jpg)

# 5  安装Pandoc

## 5.1 为什么要用Pandoc
Pandoc 是一个标记语言转换工具，可实现不同标记语言间的格式转换，堪称该领域中的“瑞士军刀”。

Typora 的文件导入/导出功能使用 Pandoc 把 Markdown 源码转换成不同的文件格式，所以我们如果想使用文件导入/导出功能，必须先安装 Pandoc。

如果不安装 Pandoc，Typora 只支持导出 HTML 和 PDF 格式的文件。

如果安装了 Pandoc ：

Typora 支持的导入文件格式: .docx, .latex, .tex, .ltx, .rst, .rest, .org, .wiki, .dokuwiki, .textile, .opml, .epub.

Typora 支持的导出文件格式 : HTML, PDF, Docx, odt, rtf, Epub, LaTeX, Media Wiki,Image.

## 5.2 macOS

macOS 有两种安装方式：使用安装包安装或使用 homebrew 安装。

1.  使用安装包安装
  STEP 1. 打开下载页面： https://github.com/jgm/pandoc/releases/latest

  STEP 2. 下载最新的安装包： pandoc-版本号-osx.pkg

  STEP 3. 双击后按照提示一步步安装

2.  使用 homebrew 安装

   在命令行中执行：

   ```
   sudo brew install pandoc
   ```


# 6  github不显示toc（目录内容）

在本地编辑Typora，使用[toc]后，目录自动显示出来，如下图

![image-20190630113302110](http://ww3.sinaimg.cn/large/006tNc79ly1g4j2al0ic3j308e077t9g.jpg)

而github却不显示，网上说是因为github不支持markdown的toc目录

![image-20190630115103286](http://ww3.sinaimg.cn/large/006tNc79ly1g4j2als9i8j30rf07xwg9.jpg)

## 6.1 解决方案

方案一：使用锚点
- [1、为什么要用ipic](#1为什么要用ipic)
- [2、ipic解决方案](#2ipic解决方案)
  * [2.1 下载ipic（仅限mac）](#21-下载ipic仅限mac)

格式如下，

![image-20190630122248182](http://ww4.sinaimg.cn/large/006tNc79ly1g4j2ic2901j30dk03i74v.jpg)

技巧：上图中，在[]中直接写标题，()的格式要怎么写呢，在github中点击后查看，如下图

![image-20190630122544661](http://ww3.sinaimg.cn/large/006tNc79ly1g4j2ictwmij30t404vmy6.jpg)

![image-20190630122609687](http://ww1.sinaimg.cn/large/006tNc79ly1g4j2idbf1kj30rs0493zz.jpg)

方案二：下载工具

1. [为 markdown 文件生成 toc 目录](https://github.com/houbb/markdown-toc/tree/release_1.0.2)

2. 用idea克隆项目

![image-20190630172312203](http://ww3.sinaimg.cn/large/006tNc79ly1g4jbkfv5xjj30c10cat9q.jpg)

![image-20190630172400789](http://ww4.sinaimg.cn/large/006tNc79ly1g4jbkgmqk3j30wf0h1wjl.jpg)

![image-20190630172434907](http://ww1.sinaimg.cn/large/006tNc79ly1g4jbkhj031j30fk03u3yx.jpg)

3. 找到需要生成toc的路径和文件

   ```java
   //这里是修改文件名的，示例是“中文名称.md"，我需要生成的md文件不叫这个名字，所以我改成了"学习使用Typora.md"
   String path = TestPathUtil.getAppRootPath("学习使用Typora.md"); 
   ```

![image-20190630172726721](http://ww3.sinaimg.cn/large/006tNc79ly1g4jbki1adjj30wf0jxn4m.jpg)



```java
//这里是修改路径的地方，我不需要root路径（root路径是存放项目markdown-doc的路径），去掉了，直接写上md文件存放的路径即可。其实emptyFile也可以去掉，因为没有用到，getAppRootPath方法直接返回了md的路径+参数
return "/Users/hubin/typoraDocument/technical-notes/typora/"+relativeTest;  
```

![image-20190630173216654](http://ww4.sinaimg.cn/large/006tNc79ly1g4jbkihidfj30wp0gjq8m.jpg)

4. 点击三角型运行程序

![image-20190630173700482](http://ww3.sinaimg.cn/large/006tNc79ly1g4jbkj1g8sj30iv04r0tj.jpg)

5. 手动修改下md文档

![image-20190630173742946](http://ww1.sinaimg.cn/large/006tNc79ly1g4jbkjeh50j30l40c3t9r.jpg)

6. 在终端中输入

```
git add -A
git commit -m"使用代码生成toc"
git push origin master
```

7. 整个文件夹进行生成（第3步-第4步是单个文件生成，现在是文件夹下的所有md文件生成）

```java
//将sub改为typora，这里只需要把你需要生成的目录写进去，比如typora
String path = TestPathUtil.getAppRootPath("typora");
```

![image-20190630175217535](http://ww3.sinaimg.cn/large/006tNc79ly1g4jc2lh8axj30ul0ctae2.jpg)

```java
//路径也要改一下，technical-notes/后面的typora去掉了，因为上图已经将sub改为typora，这里就不要重复写入
return "/Users/hubin/typoraDocument/technical-notes/"+relativeTest;
```

![image-20190630175423435](http://ww4.sinaimg.cn/large/006tNc79ly1g4jc2n6ebaj30uh0bb0xv.jpg)

