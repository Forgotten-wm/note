#git一次提交推送到多个仓库

####演示 同时提交到2个仓库 github gitee

>github为项目仓库 gitee为项目副仓库(备份仓库)

- 在github上建立项目,并复制clone链接
  - `https://github.com/Forgotten-wm/note.git`
  - 转到编译器IDE 克隆项目
- 在gitee上建立项目,并复制clone链接
  - `https://gitee.com/amnesia-wm/note.git`
- 打开项目目录的`git\config`
  - 找到`[remote "origin"]`,可以看到已经存在的一条url,与github的clone链接一致.
  - 在下面添加一条url,指向gitee准备好的仓库clone链接.
- 完成,测试 
  - 在第一次推送的时候需要登录gitee
>本项目的git的config
```
[core]
	repositoryformatversion = 0
	filemode = false
	bare = false
	logallrefupdates = true
	ignorecase = true
[submodule]
	active = .
[remote "origin"]
	url = https://github.com/Forgotten-wm/note.git
	url = https://gitee.com/amnesia-wm/note.git
	fetch = +refs/heads/*:refs/remotes/origin/*
[branch "main"]
	remote = origin
	merge = refs/heads/main
```