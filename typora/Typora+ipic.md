[TOC]

# 1、为什么要用ipic

在本地Typora插入图片的时候能正常显示，但是将编写的文档上传到GitHub上时，不显示了。是因为插入的时候，使用的本地链接路径，生成html文件的时候，img也是该路径，但是我们在本地存储的图片，在网站上是没有能力访问的。如下

![](http://ww2.sinaimg.cn/large/006tNc79ly1g4ixv99g4hj30kb0g1myo.jpg)

# 2、ipic解决方案

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

# 3、参考资料

1. [iPic - Markdown 图床、文件上传工具](https://toolinbox.net/iPic/ )

2. [Typora极简教程](https://www.jianshu.com/p/a6a6a22e9393)

# 4、iPic Mover设置上传后删除本地图片

在操作2.3时，可以将上传后删除本地图片的设置一起勾选，这里单独拿出来，是为了进行说明

![image-20190630101413952](http://ww1.sinaimg.cn/large/006tNc79ly1g4iytyj3j1j30jy0dwaaj.jpg)

# 5、安装Pandoc

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

   