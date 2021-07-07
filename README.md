# UbuntuAutoScript
Linux Auto Configuration Script- Linux 软件自动安装配置脚本


废话不多说，先来一张效果图，没图片你们肯定是不会看下去的。
简单的运行一下脚本，然后喝杯咖啡，打个游戏，做点其他事情，然后就没有然后了


![Screenshot from 2017-10-23 22-01-52.png](http://upload-images.jianshu.io/upload_images/3127217-5aba480a92e0229e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


![Screenshot from 2017-10-23 22-01-35.png](http://upload-images.jianshu.io/upload_images/3127217-259258316bcc280f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


写这个脚本的原因是因为作者手太贱，我有一颗强烈的好奇心，但是同时又有一双︿(￣︶￣)︿非常贱贱的双手，所以当作者在安装了无数个Linux发行版之后，再疲于每一次安装都需要重新安装软件，配置各种环境变量的生活，
简直苦不堪言，时间就是金钱，但是手贱喜欢换系统怎么办，
最后实在受不了了，自己写了一个自动化配置安装软件脚本


`用法`
```
正确打开命令行：
git clone https://github.com/SickoOrange/UbuntuAutoScript.git
cd UbuntuAutoScript
chmod +x setup.sh
sudo ./ setup.sh
```
> 如果你想自动配置你的github ssh 秘钥，只需要在命令上述命令后面追加 -g xxxxxxx@gmail.com即可，生成的秘钥会自动保存在桌面的github_ssh_key.txt文件中。

> sudo ./setup.sh -g xxxxxxx@gmail.com


    脚本已经在Github开源，欢迎随时
    `Start`
    `Fork`
    `Issue`
作者精力有限，所以还有什么没有想到希望大家多提意见

> Github:
> https://github.com/SickoOrange/UbuntuAutoScript



### 这个Bash Script都帮我们干了啥？

这里简单列举一下这个Bash Script的功能：

1. 更新系统的软件源
2. 针对Ubuntu16.04:
`楼主轻微桌面颜控，所以简单美观的桌面优化是必不可少的了`
   - 自动下载安装Gnome桌面
   - 自动下载安装 Dash To Dock插件 (就是类似苹果的软件栏)
   - 自动下载安装 ARC 风格主题
   - 自动下载安装 Flat Remix 扁平化图标
3. 自动配置 Node Js 以及 npm, 开箱即用
4. 自动下载配置 Oracle JDK，版本  1.8.0_151, 同时自动配置环境变量
       打开Terminal
       输入 java -version 验证是否正确安装
5. 自动安装Gradle 版本构建工具
6. 自动安装sdkman 用于管理多个软件开发套件的并行版本的工具
7. 自动安装Typora Linux版本的Markdown写作神器 
8. 安装常用小工具：
```
       Git           -- 版本控制软件
       Curl         -- 调试网络连接的小工具
       Gdebi        -- 有些deb软件不能通过默认安装器安装的, 可以试试他
       Vim          -- 不说了撸代码神器
       Unzip        -- linux解压zip压缩文件
       unrar        -- 解压rar
       jd           -- 命令行解析json工具
       kolourpaint4 -- 画图工具 
       flameshot    -- 截图工具
```
9. 自动下载安装常用的软件：
```
       Visual Studio Code
       Genymotion
       IntellijIDEA
 ```


#### 最后，时间仓促，目前就想到这么多，以后有什么需要的工具还会继续更新，如果大家有什么想法或者意见可以给我留言， 或者直接在Github上fork.

```
 07.07.2021 更新日志
 1. 快捷截图工具
```
![image](https://user-images.githubusercontent.com/21984530/124705299-06297c00-df28-11eb-8aef-4f9636b7d69f.png)
![image](https://user-images.githubusercontent.com/21984530/124705331-14779800-df28-11eb-95e4-5adc341c26a0.png)


```
 23.10.2017 更新日志
 1. 添加了网易云音乐
 2. 添加搜狗输入法
 ps: 搜狗输入法已经安装完毕，但是脚本只是帮你安装到系统了，你需要自己把搜狗输入法添加到fcitx中，如下图
```
> ![Screenshot from 2017-10-23 21-56-55.png](http://upload-images.jianshu.io/upload_images/3127217-3430d3da55a7fdfb.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

```
25.10.2017 更新日志
1. 添加了 linux 命令行 Json解析工具 jd
2. 添加了 画图板 kolour paint
3. 修复了window与ubuntu双系统，时间不同步的错误
4. 增加了自动配置github ssh
5. 添加解压rar工具
```

```
26.10.2017 更新日志
1. 添加了SDKMAN！是一个用于管理多个软件开发套件的并行版本的工具
2. 自动安装Gradle版本构建工具
```

```
29.10.2017 更新日志
1.自动安装 maven
2.自动安装 docker
    2.1 mysql image
    2.2 tomcat image
    2.3 nginx image
```

```
30.10.2017 更新日志
1.自动安装 sqliteman linux下一款轻量级数据库图形化软件
2. clementine linux下一款受欢迎的开源音乐播放软件
```


> 背景图片地址
> http://i.imgur.com/nZLDzzk.jpg

> Github地址:  
> https://github.com/SickoOrange/UbuntuAutoScript
