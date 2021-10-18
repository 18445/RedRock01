# Github手册

## 什么是Git

Git是一个分布式的版本控制系统，最初由Linus Torvalds编写，用作Linux内核代码的管理。在推出后，Git在其它项目中也取得了很大成功，尤其是在Ruby社区中。目前，包括Rubinius和Merb在内的很多知名项目都使用了Git。Git同样可以被诸如Capistrano和Vlad the Deployer这样的部署工具所使用。同样，eoe.cn客户端的源码也托管在github上。


GitHub可以托管各种git库，并提供一个web界面，但与其它像 SourceForge或Google Code这样的服务不同，GitHub的独特卖点在于从另外一个项目进行分支的简易性。为一个项目贡献代码非常简单：首先点击项目站点的“fork”的按钮，然后将代码检出并将修改加入到刚才分出的代码库中，最后通过内建的“pull request”机制向项目负责人申请代码合并。已经有人将GitHub称为代码玩家的MySpace。

在GitHub进行分支就像在Myspace（或Facebook…）进行交友一样，在社会关系图的节点中不断的连线。
GitHub 使用 git 分布式版本控制系统，而 git 最初是 Linus Torvalds 为帮助Linux开发而创造的，它针对的是 Linux 平台，因此 git 和 Windows 从来不是最好的朋友，因为它一点也不像 Windows。GitHub 发布了GitHub for Windows，为 Windows 平台开发者提供了一个易于使用的 Git 图形客户端。



### GitHub For Windows

GitHub for Windows 是一个 Metro 风格应用程序，集成了自包含版本的 Git，bash 命令行 shell，PowerShell 的 posh-git 扩展。GitHub 为 Windows 用户提供了一个基本的图形前端去处理大部分常用版本控制任务，可以创建版本库，向本地版本库递交补丁，在本地和远程版本库之间同步。微软也通过CodePlex向开发者提供 git 版本控制系统，而 GitHub 创造了一个更具有吸引力的 Windows 版本。

GitHub上已自动配置的Mac笔记本电脑，一个工具，可以转换设置Linux或Windows机器。

BOXEN是GitHub的自动化工具，设置和配置的Mac笔记本电脑软件开发[3]或其他类型的工作，正在使用他们的开发人员，律师，设计师，付货人，等。我们的想法是准备系统以自动方式和作为无差错尽可能用最少的干预工作。根据GitHub上，与一个新的开发机器上，他的Mac系统成立，并准备在30分钟内提交代码。

BOXEN的基础上收集了大量的几十个木偶模块，使设置的各种软件，如卡桑德拉，MongoDB中，Java软件中，Python和Ruby开发中，节点，JS，nginx的，Skype公司，甚至MINECRAFT。虽然机器上配备了一个预配置，每个用户都可以调整它的配置应有的作用。



## Github的使用

### 1：Github的注册

访问http://github.com/ 点击sign up，填写相关信息并注册。

### 2：Github的配置

点击自己头像，进入setting界面，进行账号的相关配置。Profile选项可以设置头像，姓名，头像，博客等。Account选项可以进行账户相关操作。Appearance选项可以更改页面风格与主题，Emoji的肤色设置。Account security选项对账号安全进行设置。Billing&plans选项对账户的账单与计划进行设置。Security log选项可以观看账户操作日志。Securit&analysis选项对账户的安全进行设置。Sponsorship log可以观看是否有人进行赞助。Emails管理邮箱设置。Notifications消息提示设置。Scheduled remindes计划提醒设置。



### 3：Github基础操作

#### 项目搜索：

在GitHub的主页上方搜索栏可以搜索项目。

#### 仓库创建：

在页面右上角头像左边有个“＋”号，在弹出的下拉选项中选择“New repository”，在创建页面中选择仓库拥有者，仓库简介，仓库名，仓库权限，初始化该仓库并建立

#### 仓库使用：

点击README.md文件，点击编辑框右上角的铅笔按钮进入编辑界面，在Edit file标签上，可以输入并更改消息并且可以在下方提交更改框中输入更改说明，点击commit changes按钮进行修改提交。你可以在主页面中左侧找到你创建的仓库并看到更改时间与内容。

#### GitHub 的下载：

对于windows用户，在http://windows.github.com下载安装。

对于Linux用户，使用 sudo yum install git指令进行安装。

#### GitHub Fork使用：

Fork 是对一个仓库的克隆。克隆一个仓库允许你自由试验各种改变，而不影响原始的项目。fork被用于去更改别人的开源项目或者使用别人的开源项目作为你自己想法的初始开发点或者进行漏洞修复。你可以向项目的拥有者提交pull requeset来提出更改项目漏洞。

进入一个项目，在头像下方可以找到Fork，点击Fork。复制fork仓库的URL，在cmd命令行中添加” `git clone URL` “指令创建本地克隆。使用`git remote -v` 将会看到fork当前配置的远程仓库(出现错误提示：`fatal: Not a git repository (or any of the parent directories): .git`  使用git init解决)。输入`git remote add upstream URL`（使你的fork与upstream同步）。

#### GitHub wach使用：

你可以对别人的项目开启Watching选项（默认为Not watching），表明你关注这个项目的所有动态，你会收到别人提交了的pull request，被别人发起了issue 等情况。如果你配置了邮箱，你的邮箱也会收到通知邮件。

#### GitHub stra功能：

你可以对你喜欢的项目添加star功能（相当于点赞），并可以点击头像，在下拉菜单中Your stars找到你之前添加star的项目。



### 4：GitHub指令学习：

#### 1：下载Git并安装：

在官网git-scm.com/downloads下载对应版本，选择推荐配置安装Git，打开Git Bash 输入`gir --version` 返回版本号说明安装成功。

#### 2：Git基础：

打开GitBash，我们可以使用 `git config --lis`t查看所有配置，使用 `git config --list --show-origin`查看所有配置与他们所在的文件。电脑在 C:\Users\用户名 目录下生成.gitconfig文件。可以使用`git config --global user.name` "用户名"配置用户名，使用`git config --global user.email` 邮箱地址 配置邮箱地址。我们可以用`git config user.name` 或 `git config user.email`查看单独的用户配置。我们可以新建文件夹，并右击，选择Git Bash Here（把该路径当作我们 Git 仓库）。

##### 2.1：git status：

查看仓库状态：我们可以使用git status命令查看当前状态（前提是该目录是一个 Git 仓库）

##### 2.2：git init:

初始化仓库：我们可以使用 git init 是仓库初始化，初始化完成后，它是一个空的 Git 仓库。此时可以用git status命令检查仓库。

##### 2.3：git add：

添加文件至仓库：在目录下的文件，我们可以根据 git add 指令，将文件添加至仓库。此时在 git status指令下提示 NO commits yet。此时我们的文件处于临时缓存区下面（可以使用 `git rm --cached` 除去这个缓存）。如果要添加目录下的全部文件，用`git add --all`。

##### 2.4：git commit：

提交缓存区的改动至本地版本库：我们可以通过 git commit -m "xxx"  指令将文件提交到Git 仓库 -m代表提交信息 “Xxx”代表提交内容。并会在本地版本库生成一个40位的哈希值，叫做commit-id。

`git commit -m “message”`，-m 参数表示可以直接输入后面的 “message” ，如果不加 -m 参数，那么是不能直接输入 message的，而是会调用一个编辑器一般是 vim 来让你输入这个 message。

`git commit --amend`，追加提交，它可以在不增加一个新的commit-id的情况下将新修改的代码追加到前一次的commit-id中

##### 2.5：git log：

显示日志：打印 Git 仓库提交日志，显示相关信息（作者、时间、信息等。）

##### 2.6：git branch：

创建分支：可以使用 git branch 查看当前所有分支（在git init默认初始化时，会提供一个主分支 master），此时*号后面的分支为我们当前所处分支，用 git branch name 新建一个名为name的分支。

##### 2.7：git checkout：

切换分支：使用 `git chekcout name` 指令，使我们当前切换到name 分支上，再次查看分支可看到我们*已从master分支上切换。我们可以使用 `git checkout -b name` ，使我们直接新建分支并自动切换到该分支上。

##### 2.8：git merge：

合并分支：切换到到主分支上后，使用`git merge name` 使把name分支的代码合并到master分支上来，在name分支成功合并后，使用`git branch -d name`删除该分支（未合并时无法执行）。如果我们要强制删除分支，可以使用 `branch -D` 指令。

##### 2.9：git tag：

标签报告：使用 `git tag name` ，我们可以新建一个名为name的标签。并可以使用`git tag` 查看所有标签，或使用`git tag name` 查看指定名字的标签。

##### 2.10 git clone：

克隆仓库：

###### 2.10.1：

git clone with HTTPS：

（不需要SSH）在 GitBash窗口，输入 `git clone URL`，就可以将仓库里的文件克隆至文件夹。

###### 2.10.2：

git clone with SSH：

（需要配置SSH）在GitHub Code-Clone下面切换至SSH的URL

输入 `git clone （SSH）URL` ，将仓库的文件克隆至文件夹。

##### 2.11 git push/git pull：

保证本地与远程的同步：`git push`：当代码有更新时，把本地代码推到远程仓库。 `git pull`：当远程仓库有更新，你需要把远程的拉到本地进行合并。(GitHub上在本地的主分支时main而非master)



### 5：SSH配置：

#### 5.1：SSH说明：

SSH是一种安全机制，可以防止本地与远程仓库连接时数据泄露，所以我们需要进行SSH配置

#### 5.2：生成SSH key：

在GitBash中 输入`ssh-keygen -t rsa`（用RSA算法生成密钥），连续三个回车（不输入密码），在`Your identification has been saved in /c/Users/Xxx/.ssh/id_rsa`
`Your public key has been saved in /c/Users/Xxx/.ssh/id_rsa.pub`位置可以找到密钥与公钥储存位置。

#### 5.3：添加SSH key：

在GitHub网页上找到setting-SSH and GPG keys，点击New SSH key，将刚才生成的id_rsa.pub的内容添加到里面。

#### 5.4：验证绑定：

在GitBash中输入 `ssh -T git@github.com`  出现`Hi Xxx! You've successfully authenticated, but GitHub does not provide shell access`.即为配置绑定完成。





