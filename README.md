Listen 1 (Chrome Extension) V1.4.0 
==========
（最后更新于2017年12月26日）

[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg)](LICENSE)

重要
----
Listen1的用户，有个坏消息希望和大家分享。Listen1最近收到了[QQ音乐的DMCA Takedown Notice](https://github.com/github/dmca/blob/master/2017/2017-11-17-Listen1.md), 主要代码库已经因为此原因而临时关闭。悲观一点看，Listen1项目可能会在今年内彻底消失。

Listen1诞生的初衷从不是和大公司的争夺版权利益，而是为了给予热爱音乐的人更好的收听体验，所以，Listen1是开源，免费的，并且不接受任何形式的捐助。正是因为有热爱音乐的Listen1的你们，Listen1才发展到今天这一步。不管结果如何，Listen1团队感谢所有支持过这个项目的人们。

在这个关系项目生死存亡的时刻，我寻求项目因为DMCA被github关闭的援助。如果有对这个比较了解如何解决的人，或者你想对这个事情发表看法和建议，可以在[issue](https://github.com/listen1/listen1_chrome_extension/issues/113)留言，或者发送邮件到 githublisten1@gmail.com。我们会尽最大努力，来守护Listen1，即使可能它即将成为历史。

缘起
----
当我发现找个想听的歌因为版权听不了，需要打开好几个网站开始搜索，来回切换让我抓狂的时候，我知道是时候该做点什么了。

妈妈再也不用担心我找不到我想听的歌了。这里包含了网易云音乐，虾米，QQ音乐的曲库，够全够大了吧。

搜歌，听歌，就用 `Listen1`。

[![imgur](http://i.imgur.com/yblr3KO.gif)]()

还有精选歌单哦。

Chrome安装
----
1. 下载项目的zip文件，在右上方有个 `Download ZIP`, 解压到本地

2. chrome右上角的设置按钮下找到更多工具，打开`扩展程序`

3. 选择 `加载已解压的扩展程序`(如果没有显示先选中`开发者模式`)，选中解压后的文件夹，完成！

Firefox打包安装
-----------
### 打包xpi文件（或在release页面下载已经打包好的xpi文件）
1. 将根目录下manifest_firefox.json替换manifest.json
2. `cd listen1_chrome_extension`
3. `zip -r ../listen1.xpi *`

### 安装
1. 打开Firefox，加载xpi文件，完成安装

更新日志
-------

`2017-12-26`

* 增加同步歌单到Github Gist功能。(特别感谢@ConstLhq提供创意和部分代码实现）


`2017-12-20`

* 增加搜索翻页功能，你可以看到更多的搜索结果了。(感谢@ConstLhq的提交）
* 增加合并歌单功能。可以快速的把其它你创建的歌曲合并到当前的歌单中了。(感谢@Dumeng的提交）

`2017-11-27`

* 修复网易云音乐歌单只显示第一首歌的Bug（感谢[@Binaryify/NeteaseCloudMusicApi](https://github.com/Binaryify/NeteaseCloudMusicApi)提供接口实现）

`2017-11-18`

* 修复版权原因无法播放歌曲时自动暂停的问题

`2017-11-17`

* 在我的歌单页面增加“打开歌单”功能，可打开支持网页的歌单链接地址。这样就可以导入你喜欢的歌单了。
* HTTP请求头部的Origin字段设置为正常网址

`2017-10-16`

* 修复QQ音乐歌单翻页显示重复的问题(感谢@Moobusy的提交)

`2017-10-03`

* 修复网易云音乐歌单无法显示的问题(感谢@Moobusy的提交)

`2017-09-14`

* 修复QQ音乐无法播放的bug

`2016-05-27`

* 增加快捷键功能（输入?查看快捷键设置）
* 支持同步播放记录到last.fm
* 增加搜索loading时的图标(感谢@richdho的提交）
* 页面标题增加显示当前播放信息
* 修复了在收藏对话框点击取消出现新建歌单的bug
* 重新组织代码文件夹结构

`2016-05-21`

* 增加歌单分页加载功能(感谢@wild-flame的提交)
* 修复关闭按钮随网页滚动的bug
* 修复点击暂停按钮会重置进度条和歌词的bug
* 修复点击歌单名称不跳转的bug
* 调整歌单水平位置居中

`2016-05-14`

* 增加firefox插件支持（感谢fulesdle的提交）

`2016-05-13`

* 增加我的歌单功能，可以收藏现有歌单，并创建自己的歌单
* 点击Listen 1和图标可以回到首页
* 标记了部分因版权无法播放的歌曲,增加版权提示
* 重构了音乐平台代码，使用统一的接口规范
* 重构了歌单接口，合并歌手，专辑和歌单接口
* 修复了阿里云歌手链接点击错误的bug


`2016-05-08`

* 增加歌词显示
* 精选歌单：添加歌单到当前播放列表，可点击跳转到原始链接
* 修复了搜索qq音乐时的乱码问题
* 修复了循环播放网易歌曲一段时间后暂停的bug
* 修复了可能导致微信公众号无法登录的bug
* 优化性能，删除了不必要的事件消息触发

`2016-05-02`

* 增加音量控制

即将到来的功能
----

* 歌单云同步（基于Gist）


License
--------
MIT
