---
title: Git配置
banner_img: 
index_img: 
date: 2020-04-01 10:34:59
categories: 
tags: 
---

## Git下载

[https://git-scm.com/download/win](https://git-scm.com/download/win)

## 查看配置

```bash
git config
```

## 配置代理

```bash
git config --global http.proxy "http://127.0.0.1:1080"
git config --global https.proxy "http://127.0.0.1:1081"
```

## 配置用户名和邮箱

```
git config --global user.name '用户名'
git config --global user.email '邮箱'
```

## 初始化

```bash
git init .
```

## 克隆仓库

```bash
git clone <url>
//指定目录下生成克隆文件
git clone <url> <path>
```

## 常用提交

```bash
git pull //拉取远程更新
git add . //添加文件到缓存
git commit -m '描述内容' //提交
git push //推送到远程

git push -f origin master //强制推送

git diff //查看更新的详细信息命令
git reset HEAD <file> //取消缓存命令
git rm //删除命令
//如果删除之前修改过并且已经放到暂存区域的话，则必须要用强制删除选项 -f
//如果把文件从暂存区域移除，但仍然希望保留在当前工作目录中，换句话说，仅是从跟踪清单中删除，使用 --cached 选项即可
git mv //移动或重命名命令
```

## 查看文件状态

```bash
git status
//暂存文件的命令：git add <文件名>
//放弃未暂存文件的修改命令：git checkout – <文件名>
//将被修改的文件暂存并提交的命令：git commit -a
```

## 分支管理

```bash
git branch //查看分支
git branch (branchname) //创建分支
git branch -d (branchname)//删除分支
git checkout (branchname) //切换分支
git merge (branchname)//合并某分支到当前分支
```

## 查看提交历史

```bash
git log
–oneline ：查看历史记录的简洁版本
–graph ：查看历史中什么时候出现了分支、合并
–reverse ：逆向显示所有日志
–author ：查找指定用户的提交日志
–since、–before、 --until、–after： 指定筛选日期
–no-merges ：选项以隐藏合并提交
```

## 标签

```bash
git tag //查看标签
git tag -a <tagname> -m '描述' //指定标签信息
git tag -s <tagname> -m '描述' //PGP签名标签
```

## 远程仓库

```bash
git remote add //添加远程仓库
git remote //查看当前的远程仓库
git fetch、git pull //提取远程仓仓库
git push //推送到远程仓库
git remote rm //删除远程仓库
```



