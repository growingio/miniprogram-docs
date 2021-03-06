# 页面分析

小程序的页面，按照场景，分为两类页面：

### 进入页：

用户进入小程序访问的第一个页面，例如用户从页面A进入小程序，跳转到页面B，A为进入页，而B不是（目前不支持带页面参数的情况）。

### 浏览页：

用户进入小程序浏览过的所有页面，例如用户从页面A进入小程序，跳转到页面B，A，B均为浏览页。

### 进入页面质量分析：

通过页面的进入量、跳出次数、每次进入页面浏览量、访问用户人均进入次数、平均进入时长（分钟）、和总进入时长，来衡量用户进入小程序的第一个页面。主要判断页面较为有效的满足了用户需求，或者吸引了用户，从而更好的引导用户在哪些页面和场景下进行分享。

**进入量**：即打开次数，按照进入页面拆分，即统计了打开小程序次数最多的第一个页面（落地页）。

**跳出次数**：用户打开一次小程序，仅有一个页面的浏览，就关闭或退出了小程序。这样会记一次跳出。跳出次数越高，

**每次进入页面浏览量**：按照进入页拆分后，指从A页面打开小程序，到关闭小程序，平均每次访问会浏览多少个页面。

**访问用户人均进入次数**：按照进入页拆分，指通过A页面打开小程序的次数/通过A页面进入小程序的访问用户量。

**总进入时长**：按照进入页拆分，指通过A页面打开小程序的访问时长的总和。

**平均进入时长**：按照进入页拆分，指通过A页面打开小程序的访问时长的总和/通过A页面打开小程序的次数。

### 浏览页关键质量指标分析

页面浏览，即指在小程序打开期间，被浏览过的页面。其中，页面浏览可以按照页面浏览量、访问用户量、退出率、页面停留时长、转发次数几个方面来进行评价。

**退出率**：退出率按照不同的页面去查看的时候，即描述的是A页面作为_退出页_的访问量/浏览过A页面的访问量。

\*退出页：用户在一次访问中访问的最后一个页面，是这次访问的退出页，也就是用户的这次访问是在这里结束的

**总页面停留时长（分钟）：**代表着在当前页面上用户停留的总时长。

**平均页面停留时长（秒）**：代表着在每次打开小程序，当前页面上用户停留的平均时长。

**转发分享按钮\_点击次数**：表示在这个页面上触发了多少次好友/群聊对话框的分享事件。

