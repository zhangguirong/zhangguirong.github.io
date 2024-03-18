### 起因

认真上班摸鱼的时候水贴水到了 [[@maxzs](https://linux.do/u/maxzs)](https://linux.do/u/maxzs)headphones [[这篇帖子 5](https://linux.do/t/topic/32438)](https://linux.do/t/topic/32438)，讲述了如何使用Github开源项目[[BlockTheSpot 3](https://github.com/mrpond/BlockTheSpot)](https://github.com/mrpond/BlockTheSpot)解锁Spotify高级版
值得注意的是此开源项目的Readme部分，解锁除下载外的所有高级功能，想要下载的佬友可以移步至本论坛 [[@nextstrain](https://linux.do/u/nextstrain)](https://linux.do/u/nextstrain)baby_bottle 的[[帖子 2](https://linux.do/t/topic/19035)](https://linux.do/t/topic/19035)

Features:

- Unlocks all premium features except downloads.
- Lives through Spotify updates. No need to patch Spotify after every update anymore.

### 痛点

长期混迹于国内QQ音乐和网易云的用户，本人喜好的歌单都在这两位手里 [[@tencent](https://linux.do/u/tencent)](https://linux.do/u/tencent) @163

如何解救我的歌单并转移至新安全屋就成为本次任务目标

任务要求尽可能不伤害人质（不损坏歌单）

### 执行过程

#### 首先：介绍本次任务的两位特工

- [[Netease-to-Youtube-or-Spotify 3](https://github.com/yueyericardo/Netease-to-Youtube-or-Spotify)](https://github.com/yueyericardo/Netease-to-Youtube-or-Spotify) GitHub开源项目，将歌单转化为文本
- [[Spotlistr 2](https://www.spotlistr.com/)](https://www.spotlistr.com/) 一个声称可以将任何内容转换为 Spotify 播放列表的优秀特工

### 第二步：打探本次任务目标所在位置

由于[[Netease-to-Youtube-or-Spotify 3](https://github.com/yueyericardo/Netease-to-Youtube-or-Spotify)](https://github.com/yueyericardo/Netease-to-Youtube-or-Spotify) 特工的作用是依赖于歌单id进行转化工作，所以我们要先定位到我们

#### QQ音乐

1. 打开qq音乐手机端
2. 点击我的
3. 选择你想要解救的单个歌单（我这里以收藏为例）点击右上角分享图标或你其他能找到的分享按钮
4. 选择分享给微信好友，然后分享给自己的小号或者文件传输助手
5. 转到微信点开你刚刚分享的连接，在右上角选择复制连接
6. 这时候你应该获得了类似于这样的一个连接https://i.y.qq.com/n2/m/share/details/taoge.html?platform=*****&appshare=*****&appversion=*****&hosteuin=*****&id=*****&ADTAG=wxfshare，其中的id=*******部分就算我们需要的id

#### 网易云音乐

1. 打开网易云音乐手机端
2. 点击我的
3. 选择你想要解救的单个歌单（我这里以收藏为例）点击右上角分享图标或你其他能找到的分享按钮
4. 选择复制连接
5. 这时候你应该获得了类似于这样的一个连接https://y.music.163.com/m/playlist?id=*****&userid=*****&creatorId=*****，其中的id=*******部分就算我们需要的id

### 第三步：请特工干活

1. 这时候你可以选择自己部署一份[[Netease-to-Youtube-or-Spotify 3](https://github.com/yueyericardo/Netease-to-Youtube-or-Spotify)](https://github.com/yueyericardo/Netease-to-Youtube-or-Spotify) 或者是选择直接打开[[在线网页 2](https://yyrcd.com/n2s/)](https://yyrcd.com/n2s/)

   <img src="https://cdn.linux.do/uploads/default/original/3X/9/5/9564855e58799e988980ba2a18ce83f25279fef9.png" style="zoom:67%;" />

2. 按照页面提示输入刚刚获得的id后等待片刻，在下面就可以复制我们的歌单了

3. 这时候请出咱们第二位特工，[[Spotlistr 2](https://www.spotlistr.com/)](https://www.spotlistr.com/) 点击“Let’s go → ”按钮，选择“Textbox to Spotify”。或者你也可以直接点击[[这个连接](https://www.spotlistr.com/search/textbox)](https://www.spotlistr.com/search/textbox)输入我们刚刚复制的文字版歌单

   <img src="https://cdn.linux.do/uploads/default/original/3X/f/8/f8a785f513cf9261274d9e5453e27bb389003fa7.png" style="zoom: 67%;" />

4. 点击Search按钮后，如果你是第一次请求这个特工协助，他会询问你安全屋登录权限。你只能选择相信他并给予相应权限。等待他搜索完成你可以看到他帮你转移的人员名单。注意这一步需要你仔细核对辛德勒名单，比如我这里他就自动选错了

   <img src="https://cdn.linux.do/uploads/default/original/3X/a/6/a6ced1cabb5eb2f2e5a5bfcb1b0fadf3951d4bc9.jpeg" style="zoom:67%;" />

5. 确认过后点击左边的创建播放列表即可

   <img src="https://cdn.linux.do/uploads/default/original/3X/3/2/325dfb3974f58626f1b1a65982fc893b53153aaa.jpeg" style="zoom:67%;" />