====1. YoukuAntiADs 支持对<font color="red">youku，ku6，iqiyi，tudou</font>视频前广告（黑屏）的过滤====
同时不排除由于15536900大神高超的技术也过滤了其他广告！
----
YoukuAntiADs 提供三种解决方案！<br>
Firefox用户推荐安装扩展或者UC脚本，效果更佳！<br>
====遇到问题请到*[http://bbs.kafan.cn/thread-1509944-1-1.html 卡饭]*或*[https://code.google.com/p/haoutil/issues/list Issues]*反馈，反馈请提供您<font color="red">使用的方案，问题具体描述，遇到问题的网址</font>！====
----
<font color="red">*GM脚本*</font>：_*[http://userscripts.org/scripts/show/119622 youkuantiads.user.js]*_<br>
支持大部分浏览器，需要安装脚本管理器<br>
Firefox请安装[https://addons.mozilla.org/en-US/firefox/addon/greasemonkey/ GreaseMonkey]/[https://addons.mozilla.org/zh-cn/firefox/addon/scriptish/ Scriptish]<br>
Chrome请安装[https://chrome.google.com/webstore/detail/tampermonkey%3Cbr%3E/dhdgffkkebhmkfjojejmpbldmpobfkfo TamperMonkey]<br>
Opera请安装[https://addons.opera.com/extensions/details/violent-monkey/ ViolentMonkey]<br>
Maxthon请安装[http://extension.maxthon.com/detail/index.php?view_id=1680 ViolentMonkey]<br>
缺点是不能同步Cookies，youku播放完后不能加载推荐视频
----
<font color="red">*UC脚本*</font>：_*[https://j.mozest.com/zh-CN/ucscript/script/92/ youkuantiads.uc.js]*_<br>
适用于Firefox<br>
安装完需要 <font color="blue">*清空缓存（必要时请重启Firefox）*</font>
----
<font color="red">*Firefox扩展*</font>：_*[https://haoutil.googlecode.com/svn/trunk/firefox/xpi/youkuantiads.xpi youkuantiads.xpi]*_<br>
自带播放器版 _*[https://haoutil.googlecode.com/svn/trunk/firefox/xpi/youkuantiads_with_player.xpi youkuantiads_with_player.xpi]*_<br>
适用于Firefox<br>
安装完需要 <font color="blue">*清空缓存（必要时请重启Firefox）*</font>
----
可以自行修改播放器地址为国内地址，地址见http://haoutil.cdn.duapp.com/ ，
但不保证可以长期使用！
<br>
<br>
<br>
<br>
<br>
<br>
=以下内容可能过期，使用前请仔细斟酌=
====2. YoukuV 提供优酷第三方播放器和播放列表反向代理功能，用于规避使用AdBlock Plus屏蔽广告时，优酷显示黑色倒计时提示====
----
~~<font color="red">由于最新AdBlock Plus规则已经放弃对优酷视频前广告的屏蔽，所以安装脚本后需要手动禁用以下规则</font><br>~~
===~~{{{@@||valf.atm.youku.com/valf?}}}~~===
----
 # 安装GM脚本 [http://userscripts.org/scripts/show/119622 YoukuAntiADs]<br>按下图修改播放器链接<br>https://haoutil.googlecode.com/svn/trunk/misc/youkuantiads.user.js.png
 # 下载 [https://haoutil.googlecode.com/svn/trunk/youkuv/binary/youkuv.7z YoukuV]<br>解压运行 youkuv.exe (推荐使用 [http://wangye.org/blog/archives/644/ SrvanyUI] 将 youkuv.exe 添加为系统服务开机运行)
----
*FAQ*
 # 优酷播放结束后报 *_数据加载失败_* 的错误
 这是由cookie的跨域问题造成的，可以使用如下方法解决：<br>
  # 在 hosts 文件中写入 {{{127.0.0.1 local.youku.com}}}
  # 将 {{{var loader = 'http://127.0.0.1:8008/loader.swf';}}}<br>改为 {{{var loader = 'http://local.youku.com:8008/loader.swf';}}}