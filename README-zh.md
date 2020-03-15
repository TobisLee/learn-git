# learn-git

这个项目是用来学习git命令的用法，以及记录哪种情况应该用哪种命令。



## git配置文件

列出当前配置：

```bash
$ git config --list
```

修改全局配置（配置文件在 `~/.gitconfig` ）：

```bash
$ git config --global user.name "xxx"
$ git config --global user.email "xxx@xxx.com"
```

修改本仓库配置（配置文件在 `<repo>/.git/config` ）：

```bash
$ git config --local user.name "xxx"
$ git config --local user.email "xxx@xxx.com"
```



## git初始化仓库

在本地仓库创建新的 `git` 仓库（在项目的根目录下创建 `.git` 文件）：

```bash
$ git init
```



## git克隆仓库

把远程项目下载到本地：

```bash
# Through SSH
$ git clone ssh://user@domain.com/repo.git

# Through HTTP
$ git clone http://github.com/user/repo.git
```



## git添加文件

添加目录下的全部文件：

```bash
$ git add .
```

添加目录下 `.py` 文件：

```bash
$ git add *.py
```



## git查看状态和不同

显示工作路径下已修改的文件：

```bash
$ git status
```

显示与上次提交版本文件的不同：

```bash
$ git diff
```

查看过去的提交：

```bash
$ git log
```

一行显示过去提交的信息简介：

```bash
$ git log --pretty=oneline
```

查看某个用户的所有提交：

```bash
$ git log --author="username"
```

谁，在什么时间，修改了文件的什么内容：

```bash
$ git blame <file>
```



## git提交

提交时调用文本编辑器添加提交信息：

```bash
$ git commit
```

提交时添加单行提交信息（不建议使用）：

```bash
$ git commit -m "commit message"
```

**永远不要修复一个已经推送到公共仓库中的提交** 



## git添加远程仓库

把本地仓库远程连接到远程仓库：

```bash
$ git remote add <remote> <url>
```

例如：

```bash
$ git remote add origin git@domain/repo.git
```



## git推送到远程

将本地仓库的改动提交到远程仓库的 `master` 分支：

```bash
$ git push origin master
```



## git分支



## git拉取合并



## git标签



## git替换本地改动