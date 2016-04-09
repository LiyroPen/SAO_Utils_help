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
| @ref suh_5-3-2 "Foobar2000"       | 不低于1.11.11 | 需安装foo\_cad\_plus插件<br>foo\_cad\_plus的下载和安装方式看@ref suh_5-3-2-1 "CAD插件安装方法"|
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

# 信息滚动显示 {#suh_5-3-1}
![](https://github.com/LiyroPen/SAO_Utils_help/tree/master/Images/5-3-1-1.jpg)<br>
在GGO桌面挂件[数字或文本]中附属于[音乐播放器数据集]的数据都可以在[更新参数]开头写上“%@%”    ，启用滚动模式。如果想在内容超过一定数目后才开启滚动模式，可以写成“%@n%”的形式，n为指定实数，如“%@10%”，表示在内容字数超过10的情况下才开启滚动。<br>
调整更新间隔可以调整滚动速度

# Foobar2000相关 {#suh_5-3-2}
支持GGO桌面挂件从Foobar2000中获取数据，通过[音乐播放器数据集]中的[CAD兼容播放器]所属数据选取显示<br>
![](https://github.com/LiyroPen/SAO_Utils_help/tree/master/Images/5-3-2-1.jpg)<br>

| 名称              | 类型   | 备注 |
| :---------------: | :----: | :----: |
| 播放进度          | 整数型 | 已播放时长，单位：秒<br>可用[条形图]、[直方图]显示，可取相反值 |
| 播放进度（格式化）| 字符串 | 格式为：“时：分：秒”  |
| 音量              | 整数型 | 可用[条形图]、[直方图]显示，可取相反值 |
| 标题              | 字符串 | |
| 艺术家            | 字符串 | |
| 专辑              | 字符串 | |

自定义：可以显示插件支持的关键词和自定义字符串并自由搭配，数据在[更新参数]填写<br>
支持的关键词如下： 

| 名称     | 关键词   | 备注        |
|:-------: | :------: | :---------: |
| 播放进度 | %pos%    | 当前播放秒数|
| 音量     | %vol%    | 最大值为100 |
| 标题     | %title%  |             |
| 艺术家   | %artist% |             |
| 专辑     | %album%  |             |

实例："%title%by%artist%"按[标题by艺术家]输出<br><br>
当Foobar2000安装了ffo\_cad\_plus后可以利用桌面网页挂件将程序目录下的SAO Utils\Plugins\Music Player Support\widget\cover demo\index.html加载显示封面。安装了ffo\_cad插件的Foobar2000需在安装了ffo\_cad\_plus后将ffo_cad卸载 <br>
设置完整后记得重启音乐播放器软件和SU软件,以确保成功设置

- @subpage suh_5-3-2-1

# Foobar2000相关-CAD插件安装方法 {#suh_5-3-2-1}
CAD插件下载地址：[https://github.com/RangerCD/foo-cad-plus/releases/download/v1.1.1/foo_cad_plus-1.1.1.fb2k-component](https://github.com/RangerCD/foo-cad-plus/releases/download/v1.1.1/foo_cad_plus-1.1.1.fb2k-component),[备用地址](http://pan.baidu.com/s/1mhwKQRu)
打开Foobar2000<br>
![](https://github.com/LiyroPen/SAO_Utils_help/tree/master/Images/5-3-2-1-1.jpg)<br>
点[参数选项]<br>
![](https://github.com/LiyroPen/SAO_Utils_help/tree/master/Images/5-3-2-1-2.jpg)<br>
点[组件]，[安装…]，选择插件文件进行安装

# 非Foobar2000、通用播放器相关 {#suh_5-3-3}
[即网易云音乐、虾米音乐、QQ音乐、酷狗音乐、千千静听（老版）相关]<br>
![](https://github.com/LiyroPen/SAO_Utils_help/tree/master/Images/5-3-1-1.jpg)<br>
相关信息的显示请[[!按自己使用的播放器选择，不要选择其他播放器里面的数据，如果想用那个播放器的数值就去使用那个播放器!]]，这些播放器能获取的信息偏少是因为目前RangerCD只能从窗口标题获取信息，若有相关接口资料欢迎联系RangerCD
设置完整后记得重启音乐播放器软件和SU软件,以确保成功设置

# 通用播放器相关 {#suh_5-3-4}
通用播放器不支持获取播放器信息，仅可尝试@ref suh_5-3-5 "控制播放器"中的方法控制播放器

# 控制播放器 {#suh_5-3-5}
在调用参数中填入某些特定的参数，可以为使用这项数据的挂件添加对播放器的控制功能，例如单击挂件暂停、单击挂件下一曲等功能就是依此实现的<br>
![](https://github.com/LiyroPen/SAO_Utils_help/tree/master/Images/5-3-5-1.jpg)<br>
各播放器支持参数如下表。若您使用的播放器不支持某项参数，请尝试利用@ref suh_5-4 "快捷键扩展"或使用通用播放器参数<br>

| 参数含义→        | 播放 | 暂停 | 上一曲 | 下一曲 | 音量加\减 | 音量加n\减n |
| :--------------: | :--: | :--: | :--:   | :--:   |  :------: |  :--------: |
| Foobar2000       | √    | √    | √      | √      | √         | √           |
| 网易云音乐       | √    | √    | √      | √      | ×         | ×           |
| 虾米音乐         | √    | √    | √      | √      | ×         | ×           |
| QQ音乐           | √    | √    | √      | √      | ×         | ×           |
| 酷狗音乐         | √    | √    | √      | √      | ×         | ×           |
| 千千静听（老版） | ×    | ×    | ×      | ×      | ×         | ×           |
| 通用播放器       | √    | √    | √      | √      | √         | ×           |
| 参数→→           | play | pause| prev   | next   | vol+\vol- | vol+n\vol-n |

注：vol+n/vol-n代表可以在vol+/vol-后带有数字，一次性调整n级音量，例如vol+5代表单击一次音量增加5<br>
示例图：![](https://github.com/LiyroPen/SAO_Utils_help/tree/master/Images/5-3-5-2.jpg)
