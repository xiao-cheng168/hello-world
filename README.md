# hello-world
The first repository.  
This is the first repository in my life, I will learn to use github and record in this repository.  
### 将一个仓库“拉”到自己的账户下，正确的操作是 Fork（分叉）。  
这个操作会在你的GitHub账户下创建一个原仓库的完整副本，你可以自由修改这个副本，并与原仓库保持关联。  
以下是详细步骤：  
核心操作：Fork（分叉）仓库  
1.找到目标仓库：登录GitHub，浏览到你想要复制的那个仓库主页。  
2.点击Fork按钮：在页面右上角，找到并点击绿色的 【Fork】​ 按钮。  
3.选择目标账户：在弹出的窗口中，选择将仓库Fork到你的个人账户下（通常默认就是你的账户）。  
4.等待完成：几秒钟后，你就会被自动跳转到位于你自己账户下的同名新仓库页面。URL会变成 https://github.com/你的用户名/仓库名。  
至此，这个仓库的完整副本（包括代码、提交历史等）就属于你了。  

### 克隆到本地电脑  
拥有了自己账户下的仓库后，你通常需要将其下载到本地电脑进行编辑：  
1.复制仓库地址：在你Fork后的仓库页面，点击绿色的 【Code】​ 按钮，复制仓库的HTTPS或SSH地址（如 https://github.com/你的用户名/仓库名.git）。    
2.在本地使用Git命令克隆：打开你的终端（命令行），使用 git clone命令。  
```bash  
git clone https://github.com/你的用户名/仓库名.git  
```

3.进入目录：完成后，会自动创建一个与仓库同名的文件夹，进入即可开始工作。`cd 仓库名`  


### 保持与上游仓库同步  
你Fork的仓库是独立副本，原仓库（称为“上游仓库”）的更新不会自动同步给你。如果你需要获取原仓库的最新改动，需要手动操作：  
#### 添加上游仓库地址（通常只需做一次）：  
```bash
git remotr add upstream https://github.com/原作者的用户名/原仓库名.git
```  
#### 拉取上游更新：
```bash
git fetch upstream
```
### 合并到你的本地分支（例如 main分支）:  
```bash
git checkout main
git merge main
```
