1. 下载 [ja-netfilter 18](https://gitee.com/ja-netfilter/ja-netfilter/releases) 的最新版和 [https://jbls.ide-soft.com 43](https://jbls.ide-soft.com/) 置顶中的 config 文件
2. 解压并覆盖 config 到 ja-netfilter 原本的 config
3. 修改IDEA的 idea.vmoptions 文件(文件在哪, Google 一下),在末尾填上

--add-opens=java.base/jdk.internal.org.objectweb.asm=ALL-UNNAMED
--add-opens=java.base/jdk.internal.org.objectweb.asm.tree=ALL-UNNAMED

-javaagent:/xxx/ja-netfilter.jar
将其中的 /xxx/ja-netfilter.jar 替换为你自己的路径

4. 打开IDEA, 填入激活码
激活 IDEA本体: 在[https://jbls.ide-soft.com 43](https://jbls.ide-soft.com/) 获取对应本体的激活码,粘贴到 Activation Code 中
激活插件: 点击[https://jbls.ide-soft.com 43](https://jbls.ide-soft.com/) 中的 All Plugins 项的按钮会获得到一段猴油(tampermonkey)脚本, 没有猴油的话就去 Google 浏览器插件商店下载,接着手动添加脚本到猴油中.
打开 [https://plugins.jetbrains.com 15](https://plugins.jetbrains.com/) 搜索你想要激活的插件, 点击 CLICK TO GENERATE ACTIVATION CODE 按钮就能得到该插件的激活码, 粘入到插件的 Activation Code 中即可