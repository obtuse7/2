 [toc]
## 创建本地版本库
1. Git GUI here 创建  （界面）
2. Git bash here 创建  （命令行）git init;
3. 乌龟创建  
## 添加文件
乌龟->添加（添加到暂存区）；  
乌龟->提交（提交到本地库）；
## 查看添加内容
乌龟->版本库浏览器；  

## 查看日志
乌龟->显示日志；
## 删除文件

1. 直接在文件夹中删除  ，删除后再提交；  
2. 乌龟->删除文件；  
3. 乌龟->删除文件保留本地副本；（删除库保留本地）

## 还原文件
乌龟->还原；
## 使用github创建一个远程仓库  
登录GitHub->New repository  
## 将本地仓库推送到远程
### SSH
创建SSH密钥及在GitHub上配置公钥：
1. 打开命令行->输入“ssh - keygen -t rsa”;  
2. 打开user->找到.ssh文件； 一个公钥（pub后缀）一个私钥；  
3. 复制私钥内容->进入GitHub设置->SSH and GPG keys->new keys->将复制的私钥粘贴到输入框；
#### 命令行方式
没有本地仓库的情况：  
git init  
git add README.md  
git commit -m "first commit"  
git remote add origin git@github.com:obtuse7/111.git
git push -u origin master  

有本地仓库的情况：  
git remote add origin https://github.com/obtuse7/111.git  
git push -u origin master
#### 乌龟方式
Git同步->选择远端仓库代号或创建一个（点击管理）->putty密钥选中私钥文件->推送；

                
### https
#### 命令行
没有本地仓库：  

>git init  
git add README.md  
git commit -m "first commit"  
git remote add origin https://github.com/obtuse7/111.git  
git push -u origin master 
 
有本地仓库：  
>git remote add origin https://github.com/obtuse7/111.git  
git push -u origin master  

#### 乌龟
Git同步->管理->URL（Github提供），不需要密钥->推送->输入GitHub账户名和密码；
## 克隆远程仓库到本地
进入远程仓库->点击clone or download->复制路径->打开命令行->输入git clone +路径；  

进入远程仓库->点击clone or download->复制路径->打开乌龟->git克隆->URL中输入路径;
