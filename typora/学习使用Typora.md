[TOC]

## 1、格式

  **粗体**、*斜体*、==高亮==、~~删除线~~、<u>下划线</u>、我是^上标^、我是~下标~、[超链接](http://www.baidu.com)

  ![图片](https://img3.doubanio.com/view/movie_poster_cover/lpst/public/p2411953504.jpg)

## 2、无序列表

  - 无序列表1
  - 无序列表2

## 3、有序列表

  1. 有序列表
  2. 有序列表

## 4、任务列表

  - [ ] 看电影
  - [ ] 听音乐
---------------------

## 5、快捷键

![image-20190630081821983](/Users/hubin/typoraDocument/technical-notes/typora/image-20190630081821983.png)

![image-20190630081915736](/Users/hubin/typoraDocument/technical-notes/typora/image-20190630081915736.png)

## 6、typora+git+github

### 6.1 在github上创建仓库

进入github官网，在个人仓库页面，新建私人仓库。

![image-20190630090250565](/Users/hubin/typoraDocument/technical-notes/typora/image-20190630090250565.png)

创建readme文件

![image-20190630090339988](/Users/hubin/typoraDocument/technical-notes/typora/image-20190630090339988.png)

### 6.2 克隆到本地

进入项目页面，克隆仓库到本地。

```
cd typoraDocument  //进入到本地仓库
git init  //本地仓库初始化
git clone git@github.com:ssxrs312/technical-notes.git   //克隆到本地仓库
```

### 6.3 本地用Typora打开并编辑

主要就是开启Typora的文件树视图。

![image-20190630091658200](/Users/hubin/typoraDocument/technical-notes/typora/image-20190630091658200.png)

然后打开你的仓库。

![image-20190630091724278](/Users/hubin/typoraDocument/technical-notes/typora/image-20190630091724278.png)

![image-20190630091752782](/Users/hubin/typoraDocument/technical-notes/typora/image-20190630091752782.png)

![image-20190630091807117](/Users/hubin/typoraDocument/technical-notes/typora/image-20190630091807117.png)

### 6.4 同步到github

```
#让本地仓库和远程仓库进行关联
git remote add origin git@github.com:ssxrs312/technical-notes.git
#进行添加和提交操作
git add -A
git commit -m"添加文件"
#将工程push到远程仓库
git push origin master
```

