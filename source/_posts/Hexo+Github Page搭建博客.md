---
title: Hexo+Github Page搭建技术博客教程
tags:
---
# Hexo+Github Page搭建技术博客教程

[【精选】超详细Hexo+Github Page搭建技术博客教程-CSDN博客](https://blog.csdn.net/qq_36580022/article/details/127964463)

### 前言

>博客有第三方平台，也可以自建，比较早的有博客园、CSDN，近几年新兴的也比较多诸如：WordPress、segmentFault、简书、掘金、知乎专栏、Github Page 等等。
> Github Page + Hexo 搭建个人博客的方式！Github Page 是 Github 提供的一种免费的静态网页托管服务，可以用来托管博客、项目官网等静态网页。支持 Jekyll、Hugo、Hexo 编译静态资源，

### 准备环境

- node和git环境

  - >准备 node 和 git 环境，
    >首先，安装 NodeJS，因为 Hexo 是基于 Node.js 驱动的一款博客框架，相比起前面提到过的 Jekyll 框架更快更简洁，因为天朝网络被墙的原因尝试过安装 Jekyll 失败而放弃了。
    >然后，安装 git，一个分布式版本控制系统，用于项目的版本控制管理，作者是 Linux 之父。如果 Git 还不熟悉可以参考廖雪峰大神的 Git 教程。
    >
    >
    >
    >本机安装的版本![image-20231019095020399](C:\Users\lmyfi\AppData\Roaming\Typora\typora-user-images\image-20231019095020399.png)

- 安装Hexo

  - > 如果以上环境准备好了就可以使用 npm 开始安装 Hexo 了。也可查看 Hexo 的详细文档。在命令行输入执行以下命令：
    >
    > ```shell
    > npm install -g hexo-cli

  - >安装 Hexo 完成后，再执行下列命令，Hexo 将会在指定文件夹中新建所需要的文件。
    >
    >```shell
    >hexo init myBlog
    >cd myBlog
    >npm install
    >```

  - >.
    >├── _config.yml # 网站的配置信息，您可以在此配置大部分的参数。 
    >├── package.json
    >├── scaffolds # 模版文件夹
    >├── source  # 资源文件夹，除 _posts 文件，其他以下划线_开头的文件或者文件夹不会被编译打包到public文件夹
    >|   ├── _drafts # 草稿文件
    >|   └── _posts # 文章Markdowm文件 
    >└── themes  # 主题文件夹

  - > 运行 hexo s 命令，其中 s 是 server 的缩写，在浏览器中输入 http://localhost:4000 回车就可以预览效果了。
    >
    > ```shell
    > hexo s
    > ```
    >
    > ![image-20231019100358458](C:\Users\lmyfi\AppData\Roaming\Typora\typora-user-images\image-20231019100358458.png)

### Github配置

> 注册好GitHub后就 new repository 创建一个新的仓库，注意点来了，Github 仅能使用一个同名仓库的代码托管一个静态站点，这个网上很多教程没说到的。

> 本人自建仓库![image-20231019100922856](C:\Users\lmyfi\AppData\Roaming\Typora\typora-user-images\image-20231019100922856.png)



### 配置SSH key

上面搭建博客有点问题：

- 补充修改手段（看评论区）：[hexo发生error：spawn failed错误的解决方法_error: spawn failed-CSDN博客](https://blog.csdn.net/qq_28919533/article/details/124338891)

> 要使用 git 工具首先要配置一下SSH key，为部署本地博客到 Github 做准备。



### Coding代码托管

国内托管平台，为了能被百度等国内平台收录自己的博客进行配置：[DevOps_DevOps 解决方案_一站式 DevOps_开发者工具 | 腾讯云 CODING DevOps](https://coding.net/)

报错解决：验证弹窗不在弹出，git bash需要管理员权限才能使用里面的第二种方法

>Coding平台用户名为手机号

[remote: CODING 提示: Authentication failed. remote: 认证失败，请确认您输入了正确的账号密码。 fatal: Authentication failed_陆慢慢的博客-CSDN博客](https://blog.csdn.net/qq_21017997/article/details/120902716)



[remote: Coding 提示: Authentication failed. remote: 认证失败，请确认您输入了正确的账号密码。-CSDN博客](https://blog.csdn.net/sunnyzyq/article/details/102471360)



### 后面的百度提交等还没做

## 扩展

- npm

  - >NPM的全称是Node Package Manager，是一个NodeJS包管理和分发工具，已经成为了[非官方](https://baike.baidu.com/item/非官方/2664029?fromModule=lemma_inlink)的发布Node模块（包）的标准。 [1]
    >
    >2020年3月17日，[Github](https://baike.baidu.com/item/Github/10145341?fromModule=lemma_inlink)宣布收购npm，GitHub现在已经保证npm将永远免费。
    >
    >npm是[JavaScript](https://baike.baidu.com/item/JavaScript/321142?fromModule=lemma_inlink)[运行时](https://baike.baidu.com/item/运行时/3335184?fromModule=lemma_inlink)环境Node.js的默认包管理器。

- Shell

  - > 在[计算机科学](https://baike.baidu.com/item/计算机科学/9132?fromModule=lemma_inlink)中，Shell俗称壳（用来区别于核），是指“为使用者提供操作界面”的软件（command interpreter，命令[解析器](https://baike.baidu.com/item/解析器/17458345?fromModule=lemma_inlink)）。它类似于[DOS](https://baike.baidu.com/item/DOS/32025?fromModule=lemma_inlink)下的[COMMAND.COM](https://baike.baidu.com/item/COMMAND.COM/8063418?fromModule=lemma_inlink)和后来的[cmd.exe](https://baike.baidu.com/item/cmd.exe/8192925?fromModule=lemma_inlink)。它接收用户命令，然后调用相应的[应用程序](https://baike.baidu.com/item/应用程序/5985445?fromModule=lemma_inlink)。

- Dos

  - >[磁盘操作系统](https://baike.baidu.com/item/磁盘操作系统/3793138?fromModule=lemma_inlink)（Disk Operating System），是早期[个人计算机](https://baike.baidu.com/item/个人计算机/3731770?fromModule=lemma_inlink)上的一类[操作系统](https://baike.baidu.com/item/操作系统/192?fromModule=lemma_inlink)。
    >
    >从1981年MS-DOS1.0直到1995年MS-DOS 6.22的15年间，DOS作为微软公司在个人计算机上使用的一个操作系统载体，推出了多个版本。DOS在IBM PC 兼容机市场中占有举足轻重的地位。可以直接操纵管理硬盘的文件，以DOS的形式运行。

    