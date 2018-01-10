# 第四章 部署到github的gh-pages分支

首先，使用```gitbook build```将书籍内容输出到默认目录，也就是当前目录下的**_book**目录

```
gitbook build
```

### 部署到 gh-pages 分支

这个步骤我使用了```gh-pages```这个工具，它可以将文件夹一键发布到 GitHub 项目下的```gh-pages```分支中（其他分支也可以发布，但是在本文下用到的就是```gh-pages```这个分支）。

首先先安装```gh-pages```工具

```
npm install -g gh-pages
```

然后在_book文件夹所在的目录使用如下命令直接发布到github的gh-pages分支

```
gh-pages -d _book
```


