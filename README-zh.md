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



## git提交



## git推送到远程



## git添加远程仓库



## git分支



## git拉取合并



## git标签



## git log



## git替换本地改动