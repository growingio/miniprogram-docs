# 获客场景

微信中开放了非常多进入小程序的入口，每次打开小程序时，GrowingIO会获取到进入小程序时的入口信息。

### 入口分布与趋势

默认统计**过去7天**小程序打开次数、获取访问用户数、获取新访问用户Top10的场景及每日趋势。右上角“自定义”可以支持选择自定义的时间。当选择“今日”时，趋势图会自动切换为今日小时颗粒度的数据。

通过打开次数、访问用户数、新访问用户数的入口分布和趋势，可以较为直观的得到用户进入小程序场景的洞察。

### 推广获客

推广获客按照GrowingIO预置的广告来源维度统计，展示**过去7天**中访问用户和新访问用户Top10的广告来源。

小程序目前支持公众号图文链接、二维码、广告等投放方式；GrowingIO可以通过识别在投放的落地链接中加入UTM参数的方式，来自动跟踪推广数据。具体可以参考[渠道跟踪](../data-analytics/channel-tracking.md)内容。

**注**：目前微信支持的小程序入口值如下：

| 1001 | 发现栏小程序主入口 |
| :--- | :--- |
| 1005 | 顶部搜索框的搜索结果页 |
| 1006 | 发现栏小程序主入口搜索框的搜索结果页 |
| 1007 | 单人聊天会话中的小程序消息卡片 |
| 1008 | 群聊会话中的小程序消息卡片 |
| 1011 | 扫描二维码 |
| 1012 | 长按图片识别二维码 |
| 1013 | 手机相册选取二维码 |
| 1014 | 小程序模版消息 |
| 1017 | 前往体验版的入口页 |
| 1019 | 微信钱包 |
| 1020 | 公众号 profile 页相关小程序列表 |
| 1022 | 聊天顶部置顶小程序入口 |
| 1023 | 安卓系统桌面图标 |
| 1024 | 小程序 profile 页 |
| 1025 | 扫描一维码 |
| 1026 | 附近小程序列表 |
| 1027 | 顶部搜索框搜索结果页“使用过的小程序”列表 |
| 1028 | 我的卡包 |
| 1029 | 卡券详情页 |
| 1030 | 自动化测试下打开小程序 |
| 1031 | 长按图片识别一维码 |
| 1032 | 手机相册选取一维码 |
| 1034 | 微信支付完成页 |
| 1035 | 公众号自定义菜单 |
| 1036 | App 分享消息卡片 |
| 1037 | 小程序打开小程序 |
| 1038 | 从另一个小程序返回 |
| 1039 | 摇电视 |
| 1042 | 添加好友搜索框的搜索结果页 |
| 1043 | 公众号模板消息 |
| 1044 | 带 shareTicket 的小程序消息卡片 |
| 1045 | 朋友圈广告 |
| 1047 | 扫描小程序码 |
| 1048 | 长按图片识别小程序码 |
| 1049 | 手机相册选取小程序码 |
| 1052 | 卡券的适用门店列表 |
| 1053 | 搜一搜的结果页 |
| 1054 | 顶部搜索框小程序快捷入口 |
| 1056 | 音乐播放器菜单 |
| 1057 | 钱包中的银行卡详情页 |
| 1058 | 公众号文章 |
| 1059 | 体验版小程序绑定邀请页 |
| 1064 | 微信连Wi-Fi状态栏 |
| 1067 | 公众号文章广告 |
| 1068 | 附近小程序列表广告 |
| 1069 | 移动应用 |
| 1071 | 钱包中的银行卡列表页 |
| 1072 | 二维码收款页面 |
| 1073 | 客服消息列表下发的小程序消息卡片 |
| 1074 | 公众号会话下发的小程序消息卡片 |
| 1077 | 摇周边 |
| 1078 | 连Wi-Fi成功页 |
| 1079 | 微信游戏中心 |
| 1081 | 客服消息下发的文字链 |
| 1082 | 公众号会话下发的文字链 |
| 1089 | 微信聊天主界面下拉 |
| 1090 | 长按小程序右上角菜单唤出最近使用历史 |
| 1091 | 公众号文章商品卡片 |
| 1092 | 城市服务入口 |
| 1095 | 小程序广告组件 |
| 1096 | 聊天记录 |
| 1097 | 微信支付签约页 |
| 1102 | 服务号 profile 页服务预览 |

\*Tip：由于Android系统限制，目前微信还无法获取到按 Home 键退出到桌面，然后从桌面再次进小程序的场景值，对于这种情况，会保留上一次的场景值。

微信文档链接：[https://developers.weixin.qq.com/miniprogram/dev/framework/app-service/scene.html](https://developers.weixin.qq.com/miniprogram/dev/framework/app-service/scene.html)

#### 

