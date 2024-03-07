[Gmeek](https://github.com/Meekdai/Gmeek) 一个博客框架，超轻量级个人博客模板，完全基于Github Pages 、 Github Issues 和 Github Actions，可以称作All in Github。不需要本地部署，从搭建到写作，只需要18秒，2步搭建好博客，第3步就是写作。

安装
安装及其简单，但是也要认真看下面的步骤，一步一步来。

点击[通过模板创建仓库](https://github.com/new?template_name=Gmeek-template&template_owner=Meekdai)，建议仓库名称为XXX.github.io，其中XXX为你的github用户名。

在你创建好的仓库的设置Settings中Pages->Build and deployment->Source下面选择Github Actions。

打开一篇issue，开始写作，并且添加一个标签（只添加一个），保存issue后会自动创建博客内容，片刻后可通过https://xxx.github.io/ 访问

配置文件
按照安装步骤成功搭建好后，就可以阅读下面的内容修改配置文件啦。
注意修改配置文件后一定要手动全局生成一次，不然会报错。

config.json 文件就是配置文件，在创建的仓库内可以找到，默认填写的是我的信息，对应修改为自己的即可。

{
    "title":"Meekdai",
    "displayTitle":"eekdai",
    "subTitle":"童话是一种生活态度，仅此而已。",
    "homeUrl":"http://blog.meekdai.com",
    "avatarUrl":"http://meekdai.com/avatar.jpg",
    "faviconUrl":"http://meekdai.com/favicon.ico",
    "singlePage":[],
    "GMEEK_VERSION":"last"
}
以上是必须的字段，下面是可以自定义字段的描述，可以选择加入到config.json中。

"email":"meekdai@163.com",
"startSite":"02/16/2015",
"filingNum":"浙ICP备20023628号",
"onePageListNum":15,
"commentLabelColor":"#006b75",
"yearColorList":["#bc4c00", "#0969da", "#1f883d", "#A333D0"],
"i18n":"CN",
"dayTheme":"light",
"nightTheme":"dark_colorblind",
"urlMode":"pinyin",
"style":"",
"script":"",
另有不清楚的也可以参考 https://github.com/Meekdai/meekdai.github.io/blob/main/config.json

常见问题
搭建不成功
多半是没有按照安装步骤来，其实搭建就这2步，不要自己乱点乱设置，就不会有问题。
案例一：https://github.com/Meekdai/Gmeek/issues/14
案例二：https://github.com/Meekdai/Gmeek/issues/18
案例二：https://github.com/Meekdai/Gmeek/issues/20

Actions执行失败
修改了config.json配置文件后，需要全局生成。另外label标签没有打，或者多打也会出现这个问题。
建议通过Actions->build Gmeek->Run workflow->里面的按钮全局重新生成一次
案例一：https://github.com/Meekdai/Gmeek/issues/1
案例二：https://github.com/Meekdai/Gmeek/issues/10

如果要导入以前的文章，如何设置发布时间呢？
如需修改发布时间，可以在文章最后一行添加如下代码。里面的时间是采用时间戳的形式，可以用如下[网站](https://tool.lu/timestamp)转换。

<!-- ##{"timestamp":1490764800}## -->
自定义单篇文章页面的style和script
<!-- ##{"style":"<style>#postBody{font-size:20px}</style>"}## -->
<!-- ##{"script":"<script async src='//busuanzi.ibruce.info/busuanzi/2.3/busuanzi.pure.mini.js'></script>"}## -->
可同时一起添加多种自定义参数：
<!-- ##{"script":"<script async src='//busuanzi.ibruce.info/busuanzi/2.3/busuanzi.pure.mini.js'></script>","style":"<style>#postBody{font-size:20px}</style>","timestamp":1490764800}## -->
添加全局文章页面的style和script
在config.json文件中添加

"style":"<style>#postBody{font-size:20px}</style>",
"script":"<script async src='//busuanzi.ibruce.info/busuanzi/2.3/busuanzi.pure.mini.js'></script>",
置顶博客文章,只需要Pin issue即可。

如果在评论里面登录后评论报错，可直接按照提示安装utteranc app即可

Error: utterances is not installed on xxx/xxx.github.io. If you own this repo, install the app. Read more about this change in the PR.