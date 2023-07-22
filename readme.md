# 杂鱼游戏类型
第三人称视角的联机对战游戏
## 开发工具
- Visual Studio 2022(默认包括在Unity安装内)
- Unity 2022.3.3f1c1 LTS
- Git(但是只有主干分支和开发分支)
## 快速安装
### 1.下载Unity(会的看一眼版本就得了)
https://unity.cn/releases/lts/2022 先点击右侧的下载Unity Hub。<br>
Unity Hub是Unity启动器，建议整一个，真的，不要单独下载。<br>
安装后，注册一下，在安装界面选择安装编辑器，选择2022.3.3f1c1，一定要一模一样，没有c1也不行。<br>
没有的话就回到上面的网站，在2022.3.3f1c1版本处，点击从Hub下载，Unity Hub就弹出来了。<br>
安装选项可以什么都不改，需要打包(不会有人不打包吧)就加个Windows Build Support(IL2CPP)，想兼容安卓啥的就也选上。下面的语言没啥大用，改了语言更看不懂，不要中译中。<br>
VS2022应该是默认安装的，有的话可能会错误，反正有就行。<br>
### 2.下载Git
自己下去，Goooogle一下，Git你还看教程。<br>
### 3.拉项目
有git就checkout一下项目吧，到了这步了记得发个邮箱加个权限，不然没有提交权限。git操作就不教了。<br>
## 项目分支
游戏分支真的太容易冲突了，尤其是啥内容都做，所以就别分支了。<br>
一个master分支发布版本，稳定的可以跑的。一个development(dev)分支用来开发。反正就是一个Release一个Debug。<br>
冲突别直接覆盖啊，做好的覆盖没了很搞心态的。<br>
## 目录介绍
Client-客户端，就是客户端。<br>
	project-Unity仓库，存放Unity项目，开的话直接开这个项目就好了。<br>
Server-服务端，就是服务端，后面记得补一下。<br>
Other-有些不属于客户端和服务端的小工具，或者一些其他类型的资源，扔这里吧。<br>

# 下面的内容是原来的杂鱼.md
## 游戏内容
### 核心玩法
游戏含有多个可选职业，玩家可根据自己的职业[^1]，进行额外属性的搭配[^2]，传入同一张地图，进行对战，另一方倒下后己方获胜，时间结束时根据剩余血量或得分方式，判决胜利。
### 其他功能[^3]
- 玩家的登录注册，服务器保留玩家数据。
- 好友和聊天功能。
- 排行/房间。
- ~~商城~~
## 开发流程
~~待定~~

[^1]:职业系|效果
|战|力血平均，低智，近战均衡系职业|<br>
|坦|高血低智，技能系更偏控制|<br>
|射|低血，远程高输出职业|<br>
|暗|力血略低，高敏捷，可以隐匿，多突进系技能，更加灵活|<br>
|术|低血高智，远程高爆发|<br>
|巫|低血高智，可对敌人造成持续性的伤害和debuff|<br>
[^2]: 一种选择是通过职业副系实现，另一种通过部分自选技能和buff，或者通过可选的武器各个数值差异实现不同。
[^3]:其他功能取决于服务器及数据库等的具体实现。
