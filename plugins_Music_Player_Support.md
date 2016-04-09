# 插件-音乐播放器支持 {#suh_5-3}
音乐播放器支持-在线最新项目页面：[http://www.rangercd.com/sao/music-player-sp-page](http://www.rangercd.com/sao/music-player-sp-page)<br>
音乐播放器支持-在线最新帮助文档：[http://www.rangercd.com/sao/music-player-sp-help](http://www.rangercd.com/sao/music-player-sp-help)<br>
***
[音乐播放器支持]插件的大部分功能需要[GGO桌面挂件]才能实现，Foobar2000的封面显示需要[桌面网页挂件]才能实现<br>
在[音乐播放器支持]插件启用时（新手不用管这），可以利用[GGO桌面挂件]和[桌面网页挂件]来显示音乐播放器中的信息和控制播放器<br>
这不是一个播放器，而是一个将你的播放器与SAO Utils互联的组件<br>
***
操作系统（OS）需求：<br>

|               | 系统位数  32位   x86 | 系统位数  64位   x64 |
| ------------- | :------------------: | :------------------: |
| Windows 2000  | √                    | ×                    |
| Windows XP    | √                    | √                    |
| Windows Vista | √                    | √                    |
| Windows 7     | √                    | √                    |
| Windows 8     | √                    | √                    |
| Windows 8.1   | √                    | √                    |
| Windows 10    | √                    | √                    |

SAO Utils需求：<br>
SAO Utils版本不低于Alpha 3/Beta 1，NERvGear版本不低于0.3.0 <br>
（SAO Utils版本在首选项中的[关于]查看）<br>
（NERvGear指的是SU根目录下的【NERvGear.dll】，可右键查看[属性]，在[详细信息]中的[文件版本]查看版本，不过SU版本没问题的话，NERvGear版本应该也是没问题的）<br><br>
播放器需求：

| 播放器名称       | 版本需求      | 备注 |
| -------------    | :-----------: | :------------------: |
| @ref suh_5-3-2 "Foobar2000"       | 不低于1.11.11 | 需安装foo_cad_plus插件<br>foo_cad_plus的下载和安装方式看[CAD插件安装方法]|
| @ref suh_5-3-3 "网易云音乐"       | 不明          |                      |
| @ref suh_5-3-3 "虾米音乐"         | 不低于2.0     |                      |
| @ref suh_5-3-3 "QQ音乐"           | 不明          |                      |
| @ref suh_5-3-3 "酷狗音乐"| 不明          |                      |
| @ref suh_5-3-3 "千千静听（老版）" | 不明          |                      |
| @ref suh_5-3-4 其他播放器       | 任意          | 支持多媒体按键       |

在上表选择相应的播放器查看相应播放器信息显示<br>
播放器信息的滚动显示看@ref suh_5-3-1 "信息滚动显示"
控制方法看@ref suh_5-3-5 "控制播放器"<br>
设置完整后记得重启音乐播放器软件和SU软件,以确保成功设置

- @subpage suh_5-3-1
- @subpage suh_5-3-2
- @subpage suh_5-3-3
- @subpage suh_5-3-4
- @subpage suh_5-3-5
