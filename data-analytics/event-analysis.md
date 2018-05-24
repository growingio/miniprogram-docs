# 事件分析

### **什么是事件？**

事件就是指用户在产品内做了什么事情，转义成描述性语言就是“操作+对象”。我们当前提供的事件类型包括：浏览页面，点击元素，浏览元素，修改文本框等。  
我们还提供了自定义事件分析，也就是对打点指标的支持。 事件分析中供选择的是指标，指标是事件的度量方式，比如对于 “点击加入购物车按钮” 这个事件，我们可以用点击次数或者点击人数来度量，对应的指标分别是 “点击加入购物车按钮的次数” 和 “点击加入购物车按钮的人数”。

### **事件分析能解决什么问题？**

1. 产品和运营同学如何才能对网站每天的 PV、UV、DAU \(日活跃用户数量\)等总体数据有一个直观的把握，包括它们的数值以及趋势？
2. 面对复杂的数据，单从数字来看，不仅效率低下，而且难以直观的发现数据背后所展现的趋势，应该怎么办？
3. 当做了第三方付费渠道推广后，运营同学如何才能有效比较不同渠道带来的流量？

   针对不同场景下的数据可视化需求，我们提供了事件分析这个功能，通过事件分析创建多样的图表来满足您不同分析场景下的数据可视化需求。

### **事件分析介绍**

事件分析提供了9种不同的图表样式，依次是：1.线图 2.横向柱图 3.纵向柱图 4.表格 5.数值 6.气泡图 7.维度线图 8.维度柱图 9.周期对比线图。创建不同的图表是提供数据可视化的重要工具之一，用户可以通过选择指标和维度，将 GrowingIO 采集到的数据进行可视化呈现。  
下面将为您分别介绍事件分析种各种图表类型以及不同的图表适用的场景。

#### **1. 线图**

可以用于观察一个或多个数据指标连续变化的趋势，也可以根据需要与之前周期进行同比数据分析。线图的横轴是系统默认的时间，纵轴是指标。点击选择具体指标，该指标的数据会依次添加到右侧的线图中。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/xian-tu-tuo-min.png)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/xian-tu-tuo-min.png)

您可以选择一个或多个指标，这些指标都会在同一个坐标轴中呈现，所以建议同张图表中的指标，数量级是类似的。  
例如：页面浏览量和访问用户量放在一起比较合适；按钮的浏览量和点击量要视情况而定，数据相差几十倍就不太合适；我们有两种数量级，量和百分比，浏览量和点击率，放在同一个坐标轴中就完全不合适。  
当您选择显示今天、昨天、以及最近7天之内的数据时，我们可以提供小时粒度的数据\(周期对比曲线图除外\)； 如果选择最近7天之外的日期时，无法展示小时颗粒度的数据，具体的颗粒度根据您选择的时间范围可调整为：天/周/月，便于您根据场景追踪具体指标随时间的变化。

#### **2. 纵向柱图**

纵向柱图主要用于观察一个或多个指标的变化趋势，产品经理和运营人员可以通过纵向柱图分析流量的走向，如每日PV，UV，DAU。您也可以比较页面浏览量和访问用户量在一段时间内的变化，就可以看出进行推广和拉新活动后的数据是否发生突变，究竟是吸引了更多新用户，还是吸引了更多现存用户回访。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/tuo-min-zong-xiang-zhu-tu-1.jpg)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/tuo-min-zong-xiang-zhu-tu-1.jpg)

纵向柱图跟线图基本类似，横坐标限定了时间维度。

#### **3. 表格**

表格是信息最密集的呈现方式，可以同时分析多指标和多维度的数据，您可以选择指标和维度，然后设置时间范围和展示粒度，可以进行维度过滤

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/biao-ge-tuo-min.jpg)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/biao-ge-tuo-min.jpg)

相较图表的形式，表格不那么容易看出变化趋势, 但是能更快地得到具体数值。对于核心KPI 或您关心的指标，快速进行多维度拆解，灵活性高。图表中最多展示100条信息，表格进行多维度拆解时往往无法完整展示所有数据，您也可以下载表格以观测完整数据。注：下载受到权限控制。

#### **4. 横向柱图**

横向柱图是一种频数图，主要用于观察某个指标在某个维度上的分布。根据业务需求对指标按照一定维度拆分，对比不同组别的频数，便于分清轻重缓急， 您可以选择指标以及维度，进行时间范围调整和维度过滤。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/heng-xiang-zhu-tu-tuo-min-1.jpg)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/heng-xiang-zhu-tu-tuo-min-1.jpg)

上图展示的是页面浏览量在不同浏览器下的分布。可以发现，横向柱图清晰展示了用户在不同类别上的频数，并且按照数量从大到小进行排序。在资源有限的情况下产品可以先适配 Chrome 浏览器以提升绝大部分用户的体验。 常用来细分的维度，如浏览器，操作系统，城市，App版本，设备型号，广告来源等。 应用：您做了渠道推广后，希望查看不同访问来源的访问用户量，可以选择指标为“访问用户量”，维度选择为“访问来源”。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/heng-xiang-zhu-tu-tuo-min-2.jpg)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/heng-xiang-zhu-tu-tuo-min-2.jpg)

可以看到上图显示的是：在过去7天内访问用户数总量前10名的访问来源按照降序显示出来，您可以判断哪些是高质量的渠道。

#### **5. 数值图**

数值表显示数据的方式最直观，当您想把您的核心指标通过最直观的形式展现时，建议使用数值表形式。选择具体的指标，对时间和维度进行选择，然后填写图表名称，保存即可。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/shu-zi-tu-tuo-min-1.jpg)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/shu-zi-tu-tuo-min-1.jpg)

数值表的数值类型为 “合计值”，上图的的意思是：在过去7天内，页面浏览量的总量为74.7万，较上周期低1.12%。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/shu-zi-tu-tuo-min-2.jpg)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/shu-zi-tu-tuo-min-2.jpg)

数值图中几类指标 “合计值”口径说明 1. 跳出率 跳出率 =在当前选择时间范围内， 只有一个页面浏览访问总个数/总访问个数 2. 平均访问时长（分钟） 平均访问时长\(分钟\)=在当前选择时间范围内，访问总时长/总访问量 3. 复合指标 若我们新建一个复合指标，如上例：新访客比例=新访问用户量 / 访问用户量，这个周期的新访客比例为0.64，含义为：这个周期的新访问用户量汇总值（去重）/这个周期的全部用户汇总值（去重）的值为0.64。

#### **6. 气泡图**

气泡图主要是分析多个事件在一个维度上之间的关系，比如油耗，速度，价格和不同的车型之间的关系。您可以分别设置X轴、Y轴的具体事件，选中具体维度，再设置大小、颜色表示的事件，对时间和维度进行筛选，然后填写图表名称，保存即可。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/qi-pao-tu-tuo-min-1.jpg)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/qi-pao-tu-tuo-min-1.jpg)

#### **7. 维度线图**

维度线图，可以快速区分这个指标在某个维度上随时间的连续变化趋势。我们提供的维度线图目前支持单指标和单维度。您可以根据您的具体需求，选择合适的指标和维度，然后设置时间范围和展示粒度，可以设置维度过滤，为了方便观测，可以选择显示合适的线条数量。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/wei-du-xian-tu-tuo-min-1.jpg)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/wei-du-xian-tu-tuo-min-1.jpg)

如果将页面浏览量按照地区维度进行拆分，那么在过去7天内，一周排名前10的地区页面浏览量连续变化曲线如上图所示。

#### **8. 维度柱图**

维度柱图，可以快速区分某个指标在某个维度下随时间的变化趋势。与维度线图一样，维度柱图目前也支持单指标和单维度。 您可以根据您不同的业务需求，选择合适维度和指标。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/wei-du-zhu-tu-tuo-min-1.jpg)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/wei-du-zhu-tu-tuo-min-1.jpg)

将页面浏览量按照地区维度进行拆分，那么在过去7天内，一周排名前10的地区页面浏览量连续变化曲线如上图所示。

#### **9. 周期对比线图**

周期对比线图，可以快速比较某一指标在当前周期和上一周期内随时间的变化趋势及不同周期间的对比，在周期对比曲线图中，我们提供天和周的显示粒度。您可以选择具体的指标和显示的颜色。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/zhou-qi-dui-bi-qu-xian-tu-tuo-min-1.jpg)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/zhou-qi-dui-bi-qu-xian-tu-tuo-min-1.jpg)

上图显示两条折线，图中灰色较暗折线为上一周期数据，较亮折线为本周期的数据。 显示的意思为：在过去7天内，页面浏览量的总数为747196，相比于上周期低1.12%。同时显示了具体每天的数据量及与上周期的对比情况。

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/zhou-qi-dui-bi-qu-xian-tu-tuo-min-2.jpg)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/zhou-qi-dui-bi-qu-xian-tu-tuo-min-2.jpg)

对不同类型的指标，右上角的汇总方式的解释： 也以上面的复合指标“新访客比例”为例，下图显示了本周期（过去7天）的新访客比例为0.64，较上周的新访客比例高2.58%，同样地，新访客比例=新访问用户量 / 访问用户量，逻辑为：这个周期的新访问用户量汇总值（去重）/这个周期的全部用户汇总值（去重）。

#### **“上一周期”计算逻辑：**

根据您选择的时间范围天数，时间范围 / 7=n...m，商为n，余数是 m；若选择“过去90天”，就是90除以7，可以得到一个通用公式：

* 若 n &lt; 1，上一周期对比为上周的周同比，举例来说这周四对应的上周期就是上周四；
* 若 n &gt; 1， 若 m = 0，则上一周期为n周前，对比指的是 n 周前的周同比；
* 若 m &gt; 0，则上一周期为（n+1）周前，对比指的是\(n+1\)周前的周同比；

  举个具体的例子：假设现在是2017年11月30日上午11点，周四，选取的时间范围都为“相对时间为例”，得到的“上一周期”如下表所示：

  [![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/zhou-qi-dui-bi-shuo-ming.jpg)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/zhou-qi-dui-bi-shuo-ming.jpg)

#### **单图列表**

单图列表中包含了在项目下被创建的所有单图，当前包括事件分析、漏斗分析、留存分析三种图表。 在这个界面中，您可以管理您创建的图表和您有权限查看的所有图表，分别对应了”我的”和 “全部” tab。您可以在网格视图和列表视图下切换满足不同的需求，您可以进行的管理包括： 1. 发起新建图表； 2. 针对已有图表，查看图表详情并编辑\(该操作受权限控制\)图表； 3. 为图表设置权限\(该操作受权限控制\)； 4. 删除某个图表\(该操作受权限控制\)； 5. 将图表添加到某个看板中，我们鼓励您将感兴趣的图表放到自己的看板中，构建成有业务价值的看板统一监控和分析； 为了方便您快速地找到目标看板，我们提供了搜索功能供您快速查找，搜索框支持的查找范围包括：看板名称、创建人，并支持模糊搜索。

**单图列表的几个功能说明：** 1. 搜索框：在搜索框里面您可以输入单图的名称或者创建人进行搜索 2. 展示形式：可以选择是以网格还是列表的形式展示单图 3. 排序：可以用默认形式或者选择按名称，修改时间，创建时间的顺序来展示

[![](https://github.com/growingio/help_site/raw/master/.gitbook/assets/dan-tu-lie-biao-1.png)](https://github.com/growingio/help_site/blob/master/.gitbook/assets/dan-tu-lie-biao-1.png)

