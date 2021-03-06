
#### git的基础知识
> git是一个分布式代码版本管理控制系统
> - 记录当前的产品代码的所有版本信息（历史修改信息），而且方便快速回滚到某一个具体的版本
> - 方便团队协作开发，能够检测代码冲突，合并代码等

`svn`集中式管理，git之前诞生的版本控制系统
> 需要本地和中央服务起保持网络连接，这样才可以随时查看或者管理历史版本信息
[集中式管理]![Alt text](./1523351453597.png)


`git`分布式管理
 > 每个开发者在自己的本地都是一个git仓库 
1. 在本地就可以生成历史版本

 [分布式管理]![Alt text](./1523351470219.png)


#### CDN
地域式服务器分布管理

课后思考：
**git和svn的区别：**
1. 集中式和分布式核心区别；
2. 上传速度不一样，git用元数据的方式传输更快
详细解说：
- **GIT把内容按元数据方式存储，而SVN是按文件：**
	所有的资源控制系统都是把文件的元信息隐藏在一个类似.svn,.cvs等的文件夹里。如果你把.git目录的体积大小跟.svn比较，你会发现它们差距很大。因为,.git目录是处于你的机器上的一个克隆版的版本库，它拥有中心版本库上所有的东西，例如标签，分支，版本记录等。
- **GIT分支和SVN的分支不同：**
分支在SVN中一点不特别，就是版本库中的另外的一个目录。如果你想知道是否合并了一个分支，你需要手工运行像这样的命令svn propget 
- **GIT没有一个全局的版本号，而SVN有：**
目前为止这是跟SVN相比GIT缺少的最大的一个特征。
- **GIT的内容完整性要优于SVN：**
GIT的内容存储使用的是SHA-1哈希算法。这能确保代码内容的完整性，确保在遇到磁盘故障和网络问题时降低对版本库的破坏。

