什么是Git？

Git是一个开源的分布式版本控制系统，可以有效、高速地处理从很小到非常大的项目版本管理。

什么是Github？

GitHub是一个面向开源及私有软件项目的托管平台，因为只支持git 作为唯一的版本库格式进行托管

简单理解Git：

当玩单机游戏时，保存游戏，并且读取存档时能读取不同时间各个存档

简单理解Github：

当玩完steam游戏后，游戏存档会上传到steam云存档

**本地库初始化**

```html
git init
```

执行完此命令后会在本地工作区生成一个.git文件夹。里面存放着是本地库相关的子目录和文件，不要删除，也不要胡乱修改。

执行完此命令后会在本地工作区生成一个.git文件夹。里面存放着是本地库相关的子目录和文件，不要删除，也不要胡乱修改。

**设置签名（第一次必须在终端运行）**

```html
git config  user.name 'qwamvcpu'
git config  user.email 'c15940908593@163.com'
```

**状态查看**

```html
git status #查看工作区、暂存区状态
```

添加

```html
git add [file name] #将工作区的“新建/修改”添加到暂存区
```

提交

```html
git commit -m "commit message" [file name]  #将暂存区的内容提交到本地库
```

查看历史记录（时间）

```html
git log                    #查看版本历史记录（方式一）
git log --pretty=oneline   #查看版本历史记录（方式二）
git log --oneline          #查看版本历史记录（方式三）
git reflog                 #查看版本历史记录（方式四）
```

**本地库与远程库建立连接**

```
# 查看仓库
git remote -v
```

```
# 删除远程仓库
git remote rm gitee
git remote rm github
```

