# 第二节 gitbook使用

现在就可以使用gitbook命令来直接生成gitbook书籍框架，选择一个生成框架的位置

> 在本地的github仓库中直接构建gitbook框架，后续可以使用github进行维护

## 生成gitbook框架

使用如下命令生成github框架，执行该命令会在当前目录生成两个文件**README.md**和**SUMMARY.md**

* README.md:相当于一本gitbook的简介
* SUMMARY.md:相当于一个gitbook的目录结构

```
gitbook init
```

## 编辑SUMMARY.md

首先编辑SUMMARY.md文件，插入如下内容举例

```
* [简介](README.md)
* [第一章](chapter1/README.md)
    * [第一节](chapter1/section1.md)
        * [第一小节](chapter1/section1/section_min1.md) 
        * [第二小节](chapter1/section1/section_min2.md) 
    * [第二节](chapter1/section2.md)
        * [第一小节](chapter1/section2/section_min1.md) 
        * [第一小节](chapter1/section2/section_min2.md) 
* [第二章](chapter2/README.md)
    * [第一节](chapter2/section1.md)
    * [第二节](chapter2/section2.md)
* [结束](end/README.md)
```

##根据SUMMARY.md重新生成架构

根据我们编辑完成的SUMMARY.md文件，再次执行如下命令，gitbook会为我们生成新的架构

```
git init
```

我们可以看到，gitbook给我们生成了与SUMMARY.md所
对应的目录及文件。每个目录中，都有一个README.md文件，相当于一章(节或小节)的说明。

现在就可以正式编写每个章节了


