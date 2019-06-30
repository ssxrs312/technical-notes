# 目录

  * [1、格式](#1、格式)
  * [2、无序列表](#2、无序列表)
  * [3、有序列表](#3、有序列表)
  * [4、任务列表](#4、任务列表)
  * [5、快捷键](#5、快捷键)
  * [6、typora+git+github](#6、typoragitgithub)
    * [6.1 在github上创建仓库](#61-在github上创建仓库)
    * [6.2 克隆到本地](#62-克隆到本地)
    * [6.3 本地用Typora打开并编辑](#63-本地用typora打开并编辑)
    * [6.4 同步到github](#64-同步到github)




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

![image-20190630081821983](http://ww1.sinaimg.cn/large/006tNc79ly1g4iy3s797aj30r50hutg7.jpg)

![image-20190630081915736](http://ww1.sinaimg.cn/large/006tNc79ly1g4iy3t2xe5j30qt0din1z.jpg)

## 6、typora+git+github

### 6.1 在github上创建仓库

进入github官网，在个人仓库页面，新建私人仓库。

![image-20190630090250565](http://ww3.sinaimg.cn/large/006tNc79ly1g4iy3tfm8jj30ls0i9goq.jpg)

创建readme文件

![image-20190630090339988](http://ww4.sinaimg.cn/large/006tNc79ly1g4iy3ty6vuj30ry07xq5b.jpg)

### 6.2 克隆到本地

进入项目页面，克隆仓库到本地。

```
cd typoraDocument  //进入到本地仓库，本地创建typoraDocument文件夹
git init  //本地仓库初始化，在typoraDocument仓库中初始化，完成后本地仓库typoraDocument就有了
git clone git@github.com:ssxrs312/technical-notes.git   //克隆到本地仓库
```

### 6.3 本地用Typora打开并编辑

主要就是开启Typora的文件树视图。

![image-20190630091658200](http://ww1.sinaimg.cn/large/006tNc79ly1g4iy3ucfbrj30h80ac79n.jpg)

然后打开你的仓库。

![image-20190630091724278](http://ww1.sinaimg.cn/large/006tNc79ly1g4iy3utcuuj30il0ghaas.jpg)

![image-20190630091752782](http://ww1.sinaimg.cn/large/006tNc79ly1g4iy3ves1hj30hs09wgp8.jpg)

![image-20190630091807117](http://ww2.sinaimg.cn/large/006tNc79ly1g4iy3vv8stj30hw0ga75u.jpg)

### 6.4 同步到github

```
#让本地仓库和远程仓库进行关联(必须进入到本地的cd technical-notes的目录下)
git remote add origin git@github.com:ssxrs312/technical-notes.git
#进行添加和提交操作
git add -A
git commit -m"添加文件夹typora"
#将工程push到远程仓库
git push origin master
```

