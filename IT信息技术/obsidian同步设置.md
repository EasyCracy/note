### 一、git同步

详细步骤如下：
1. GitHub上创建一个仓库，或使用已有的仓库；
2. 电脑、手机安装git；
3. 在github生成`personal access token`；
4. 安装obsidian第三方插件==Obsidian Git==；
5. 创建一个目录存储远程仓库；
6. 使用命令git clone，输入远程仓库的HTTP链接（注意：带个人token）
7.  重启Obsidian

#### 1. 安装git

电脑直接访问[git官方网站](https://git-scm.com/)进行下载安装；
手机需要下载==termux==软件；

**1）termux安装git：**
```
pkg update
pkg install git
```
**2）设置termux权限**
```
termux-setup-storage
```

#### 2. github生成个人token

- 在GitHub任何页面的右上角，点击你的头像，然后点击**设置**。
- 在左侧边栏，点击**开发者设置**
- 在左侧边栏，个人**访问令牌**下，点击**令牌（经典版）**
- 选择生成新token，记住生成的token，ghp_XXXX的一串密钥，改密钥只能查看一次，忘记只能重新生成

#### 3. 安装Obsidian Git
在obsidian软件打开设置，点击第三方插件，关闭安全模式后搜索git进行下载

#### 4. 创建存储目录
在电脑或手机的obsidian上新建一个笔记仓库，命名为==git同步==。

#### 5. 拉取远程仓库
复制远程仓库的http链接，如`https://github.com/EasyCracy/note.git`，在这个链接的基础上添加github仓库的个人token，如
```
https://ghp_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX@github.com/EasyCracy/note.git
```

#### 6. 重启obsidian
拉取远程仓库完成后重启obsidian