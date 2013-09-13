如果大家有兴趣了解使用一下git，可以搜搜网上的教程或者Git Book.
对于码农来说，这是一个特别好的版本控制系统，个人认为比svn要好太多。

首先你需要安装一个可以用的git，安装以后在终端（command/Terminal）里面输入git命令如果没提示命令错误就说明已经安装好了。

git把一个项目叫做一个仓库，我们这个项目目前就是一个仓库，这个仓库的地址是https://github.com/pfctgeorge/math4ever.git。
大家可以先fork这个仓库，右上角Fork按钮。
然后你fork来的仓库会有这个仓库当前的所有内容，这时候可以把你fork来的仓库取回到你的电脑上，你可以使用如下的命令
   git clone https://github.com/{your_username}/math4ever.git

clone以后你当前目录下面就会有一个math4ever的文件夹，这个文件夹里面就是你fork来的仓库的所有内容。
先运行这个命令 git remote add upstream https://github.com/pfctgeorge/math4ever.git
你可以理解为你的仓库的父仓库是pfctgeorge/math4ever.git

然后你可以修改通讯录的有关信息，记得保存。
修改以后运行这个命令
git add <file-name>
git commit -m "你的修改信息/理由" （注意这个信息必须要有）
然后git push origin master

这时候打开网址github.com/{your_username}/math4ever.git就能看到你这次更新的结果。

但是你并没有跟最终发布的父仓库进行同步，也就是还没有与发布的版本进行合并。
这时候在网页右侧点击Pull Request -> New Pull Request就可以发一个申请，表示你更新了信息希望合并到发布的版本里面去。发了Pull Request以后我（可能将来这个父仓库的管理者会有更多）就会收到提醒，如果没有问题的话我就会Merge你的申请。这样打开github.com/pfctgeorge/math4ever.git这个仓库就可以看到你的修改真正同步到发布版本的通讯录了。

如果你想获取其他人最新的联系方式到你的本地，只需要运行命令git pull upstream master就可以了，这样本地仓库里面会把父仓库的最新内容同步下来。

PS.合作编辑的特点就是有可能带来冲突(Conflict)，为了大家更便捷的修改自己的信息。请不要修改其他人的文件，在你对git没有啥概念的时候。

OK，最简单的教程完了。

git的强大之处远不仅于如此，他能在大型仓库里面发挥更大的作用。大家有空的话慢慢研究吧。


-- Jianjin
