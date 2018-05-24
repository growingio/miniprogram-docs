# 漏斗分析

漏斗是衡量转化效果、进行转化分析的重要工具，GrowingIO 的漏斗功能够帮助您清晰地了解转化情况，从多角度剖析对比，定位流失原因，提升转化表现。

数据需要传输时间，从您传输数据到在漏斗中可用会有一定的延迟，具体情况如下：

* 打点事件：您成功发送打点事件1小时后，可以在漏斗分析中使用该事件创建漏斗；
* 圈选事件：
  * 元素浏览：圈选后第2天可用来创建漏斗，数据有效期从圈选第2天开始；
  * 页面浏览、元素点击、输入框变更等：圈选1小时后可用来创建漏斗，请注意：圈选事件回溯7天，使用新圈选事件创建漏斗时请合理选择漏斗的时间范围。
* 我们在漏斗分析中提供了一键创建分群的功能，可以快速定位转化和未转化（流失）用户，打通分析到运营环节。鼠标点击在柱状视图即可出现以下效果。当前钻取有2个限制条件需要注意：
  * 当前仅支持您保存之后进行钻取
  * 钻取创建分群受到用户分群模块权限限制，如果您没有用户分群权限，将无法钻取创建分群。

    [![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/lou-dou-yi-jian-chuang-jian-fen-qun.png)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/lou-dou-yi-jian-chuang-jian-fen-qun.png)

### 使用场景和案例

#### 案例1：「GrowingIO」发现短信验证服务停止导致注册转化率下降

我们建立了注册转化漏斗，度量了每一步的转化率和整体的注册转化率。除了看到整体的转化情况，我们按照时间维度来监控每一步和整体转化率的趋势。发现，第一步转化率在4月8日有明显下跌。 ，而该环节对应的是填写手机验证码的环节。  
经查发现，欠费导致短信验证服务被代理商自动停止，于是及时充值，恢复短信验证服务后转化率回到之前的水平。这个案例中，通过对每一步转化率的监控可以及时发现问题，及时止损，避免造成更大范围的影响。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/skitch.png)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/skitch.png)

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/2%20%281%29.png)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/2%20%281%29.png)

#### 案例2：电商平台APP购买转化率低于网站优化后明显提升

某电商网站使用 GrowingIO 漏斗衡量交易转化时发现，APP上的用户量高于网站，但转化率却低于网页端。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/3%20%287%29.png)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/3%20%287%29.png)

具体步骤上可以看出，用户提交订单之后到支付环节的转化率明显低于网页端，值得注意的是，提交了订单的用户购买意愿非常强烈，是很有潜力唤回的一批用户。但是他们却选择了返回到上一步，而不是去支付。  
对比网站和 APP 在支付页面的信息结构发现，APP上的支付页面缺少了订单商品的详细描述、收货人地址和联系方式等信息，导致很多用户返回到上一步确认，同时带给了用户犹豫，从而导致转化率下降。  
于是，产品经理参考网站的信息结构，补充了详细信息，同时在支付环节进行流失用户召回。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/4.png)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/4.png)

从漏斗的趋势图中监测支付环节优化后的效果，APP端提交订单到支付环节的转化率明显提升，甚至略高于网站转化率，整体转化率也被拉高。同时，在漏斗中选择进行召回的用户作为目标用户，观测召回后的转化率变化，以此来评估本次唤回活动的效果。  
类似转化问题，仅靠直觉是很难发现；它需要产品或者运营人员高度的数据敏锐感、娴熟的业务技能，这也是转化分析高级阶段的表现，发现问题后进行产品优化，然后回到漏斗中监控优化效果，产品在不断的迭代中，稳步增长。

### 建立你的第一个漏斗

#### 简单漏斗创建

1.从“分析”页面，选择“漏斗”，进入漏斗创建页面。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/ldbz1.png)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/ldbz1.png)

2.选择漏斗步骤：选择至少2个步骤，点击确认，至此您就可以看到漏斗视图了； 漏斗的步骤可以通过拖拽调整。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/ldbz2.png)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/ldbz2.png)

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/ldbz3.png)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/ldbz3.png)

3.漏斗的设置及默认条件包含：

* 目标用户：默认是“全部访问用户”，可以切换至“新访问用户”、“全部登录用户”、“新登录用户”以及用户自主创建的用户分群。比如要分析新用户的注册行为，可以设定目标用户为『新访问用户』。
* 过滤条件：默认不加过滤，这里针对漏斗的第一步进行过滤。比如，如果想要看使用 Chrome 浏览器发起注册的转化漏斗，就可以将过滤条件设置为：浏览器＝Chrome
* 时间：默认是“过去14天”，可以在此处切换成“今天”或者过去的一段时间。此处时间限定的是漏斗第一步，也就是用户进入转化漏斗的时间范围。
* 转化周期：默认是“1天”，最长支持90天。 比如，转化周期设置为7天，是指用户完成漏斗第一步之后，需要在后续的7天内完成漏斗的最后一步才计为转化，否则会记为流失。

4.填写漏斗名称并保存：漏斗名称最长限定25个字，输入名称后点击“保存”。至此您就完成了单一漏斗的创建。保存的漏斗可在『单图』列表中查看和管理。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/ldbz6.png)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/ldbz6.png)

#### 创建对比漏斗

1. 维度对比：针对某个维度，可以对比不同维度值的漏斗表现。举例来说，我们可以对比『浏览器』维度，Chrome 和 Safari 的注册流表现是否有明显差异。Chrome 和 Safari 是『浏览器』维度的2个不同的值。可以看到两个浏览器在注册每一步的不同表现和整体转化率的不同表现，并且可以在右侧视图区域切换『趋势』对比它们的趋势情况。
2. 用户对比：可以对比两个不同的用户群体的转化情况。举例来说，某电商平台尝试唤醒近期不活跃的用户，并将用户分成2组，其中1组发了满减优惠券，另外1组发了立减优惠券，想要2组领取了优惠券之后的转化情况；此时可以创建2用户分群：『领取了满减券的用户』\(2010人\)和 『领取了立减券的用户』\(1080人\)，在漏斗用户对比时选择这2个用户分群并调整时间范围到用户领取优惠券之后的一段时间，就可以对比2个不同用户分群的转化情况了。

[![image](https://camo.githubusercontent.com/79c8cab00a1b9e031a24da15fdb305eefa9cf940/687474703a2f2f67726f77696e672e636e2d626a2e7566696c656f732e636f6d2f3166756e6e656c2e676966)](https://camo.githubusercontent.com/79c8cab00a1b9e031a24da15fdb305eefa9cf940/687474703a2f2f67726f77696e672e636e2d626a2e7566696c656f732e636f6d2f3166756e6e656c2e676966)

#### 使用自定义（打点）事件创建漏斗

漏斗中的可选事件，包括了圈选事件和打点事件，可以在同一个漏斗分析不同步骤中同时使用圈选和打点事件；除了上述案例中演示的对所有步骤同时过滤的方法外，漏斗分析支持对每个步骤单独添加过滤条件。

1. 圈选事件可用事件类型包括：页面浏览、元素浏览、元素点击、输入框修改；4种类型。可以通过事件选择控件中的「类型」tab下拉快速选择。
2. 打点事件，在「类型」中选择“自定义事件”即打点事件。
3. 每一步添加过滤：被选中的事件会同步出现一个filter icon，点击即可对该事件进行单独的过滤。比如，我们想要选择某个步骤为「保存漏斗成功」，并且要求「漏斗步骤长度 = 3」。那么我们可以先选择事件「保存漏斗成功」，然后点击过滤icon，选择该变量「漏斗步骤长度」，大小关系设置为 = 3。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/shi-jian-lei-xing.png)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/shi-jian-lei-xing.png)

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/mei-yi-bu-tian-jia-guo-lv-shi-li.png)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/mei-yi-bu-tian-jia-guo-lv-shi-li.png)

### 漏斗内容解读

1. GrowingIO 的漏斗基于用户行为分析，漏斗每一步的数据统计的是“人数”，也就是每一步有多少人完成；如果同1个用户在选定的时间范围完成了某个步骤2次，算作1 \(单位：人\)。
2. 漏斗步骤之间的时序和计算关系：GrowingIO漏斗支持的时序是按天的时序，以漏斗第一步和第二步为例：
3. 如果用户先完成第一步又完成第二步，则第二步用户量+1；
4. 如果用户先完成了第二步然后完成了第一步，且在同一天完成，则第二步用户量+1；
5. 如果用户先完成了第二步然后完成了第一步，且不是在同一天完成（第一步是在完成第二步的后续日期完成），第二步用户量+0
6. 时间：右上角的『时间』确切是指用户进入漏斗的时间范围，也就是完成漏斗第一步的时间。举例来说，如果时间选择『6月1日~7日』，转化周期选择7天，如果1个用户在6月6日完成漏斗第一步，6月10日（转化周期为5天）完成了漏斗最后一步，那么判定该用户完成了漏斗转化。
7. 转化周期：指用户从漏斗第一步到完成漏斗最后一步需要在转化周期时长内完成记作转化，否则记作流失。转化周期以自然日计算，最小颗粒度为天；具体举例，如果用户6月1日完成漏斗第一步且当天完成最后一步，转化周期为1天，如果6月2日完成最后一步，转化周期为2天；6月1日 00:00 还是 6月1日 23:59 在计算时统一处理成 6月1日，忽略时分。
8. 过滤条件：过滤条件对漏斗第一步的事件生效。举例来说，如果1个用户上午在『北京』完成了漏斗第一步，下午在『上海』完成了漏斗最后一步，当我们使用过滤条件『城市=北京』来过滤漏斗时，漏斗第一步人数+1，最后一步人数+1；使用过滤条件『城市=上海』过滤时，第一步人数+0，最后一步人数+0。也就是说，漏斗针对第一步行为生效，通过过滤条件定位到第一步的用户之后，后续的步骤会继承第一步的用户，判断用户是否发生了漏斗后续步骤的行为，而不再做过滤条件的判定。

### 漏斗使用 Tips

1. 选择漏斗步骤时，鼠标hover在某个事件时，可以看到该事件的定义和过去7天的数据预览。

   [![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/ldbz7.png)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/ldbz7.png)

2. 在漏斗视图界面，鼠标点击事件提示icon时，可以看到该时间在选定事件周期内自身的数据情况，辅助您判断漏斗转化数据是否受到事件数据有效性的影响。举例来说，您在6月7日圈选了某个事件A，数据回溯7天，事件A的有效期是从6月1日开始的；如果您在漏斗中使用了事件A，并且时间选择了『5月20日至昨天』，其他事件的有效期从5月1日开始，而事件A是从6月1日开始；您需要注意到，漏斗的转化率数据受到了事件A有效期的影响。

   [![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/ldbz8.png)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/ldbz8.png)

### 常见问题

#### 1. 漏斗的步骤之间有时序么？

漏斗步骤之间的时序和计算关系：GrowingIO 漏斗支持的时序是按天的时序，以漏斗第一步和第二步为例，如果用户先完成第一步又完成第二步，则第二步用户量+1；如果用户先完成了第二步然后完成了第一步，且在同一天完成，则第二步用户量+1；如果用户先完成了第二步然后完成了第一步，且不是在同一天完成（也就是第一步是在完成第二步的后续日期完成），第二步用户量+0。

#### 2. 转化周期是什么意思？

用户从漏斗第一步到完成漏斗最后一步会耗费一定时长，如果该时长小于等于转化周期则记为转化，否则记作流失。转化周期以自然日计算，最小颗粒度为天；具体举例，如果用户 6月1日完成漏斗第一步且当天完成最后一步，转化周期为1天，如果 6月2日完成最后一步，转化周期为2天；6月1日 00:00 还是6月1日 23:59，计算时统一处理成 6月1日，忽略时分。

