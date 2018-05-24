# 自定义事件和变量

#### 自定义事件

手动发送一个自定义事件。在添加所需要发送的事件代码之前，需要在 GrowingIO 产品的`自定义事件和变量`管理页面配置事件以及事件级变量。

接口定义：

```javascript
gio('track', eventName: string, properties: object)
```

参数说明：

| 参数名称 | 参数类型 | 是否必须 | 说明 |
| --- | --- | --- |
| eventName | string | 是 | 事件标识符 |
| properties | object | 否 | 事件级变量，即事件发生时所伴随的维度信息参数 |

示例：

```javascript
// 假设初始化后把 gio 对象放在 App 的 globalData 里面
getApp().globalData.gio('track', 'clickBanner', { 
  id: movie.id, 
  title: movie.title, 
  index: e.currentTarget.dataset.index 
});
```

#### 用户级变量

给注册用户附上额外的信息，便于后续做用户信息相关分析。在添加所需要设置的用户变量的代码之前，需要在 GrowingIO 产品的`自定义事件和变量`管理页面配置用户级变量。

接口定义：

```text
gio('setPeople', properties: object)
```

参数说明：

| 参数名称 | 参数类型 | 是否必须 | 说明 |
| --- | --- |
| properties | object | 是 | 用户级变量，用户额外的信息参数 |

示例：

```javascript
// 假设初始化后把 gio 对象放在 App 的 globalData 里面
getApp().globalData.gio('setPeople', { 
  age: 30, 
  level: '高级用户', 
  company: 'GrowingIO', 
  title: '工程师'
});
```

#### 页面级变量

给当前页面附上更多的页面信息，可以作为维度拆分数据做分析。设置了页面级变量以后，这个页面的指标以及这个页面的行为指标，都可以继承使用这些维度信息做分析。在添加所需要设置的页面变量的代码之前，需要在 GrowingIO 产品的`自定义事件和变量`管理页面配置页面级变量。

接口定义：

```text
gio('setPage', properties: object)
```

参数说明：

| 参数名称 | 参数类型 | 是否必须 | 说明 |
| --- | --- |
| properties | object | 是 | 页面级变量，页面额外的信息参数 |

示例：

```javascript
// 假设初始化后把 gio 对象放在 App 的 globalData 里面
getApp().globalData.gio('setPage', { 
   pageName: '电影列表页', 
   type: this.data.type
});
```

#### 转化变量

高级功能，设置一个转化信息用于高级归因分析，目前支持归因方式有最初归因、最终归因和线下归因。举个例子，如果一个用户是先后通过`活动A`、`活动B`、`活动C`来访问小程序，最后在某次后续几天后的访问购买了某个商品。如果把活动A/B/C分别设置为转化变量`campaign`的值，那么如果采用了最初归因，那么这个购买行为是由 A 贡献的；如果是最终归因，那么这次购买行为是 C 贡献的；如果是线性归因，那么这次购买行为是 A/B/C 各占 1/3 贡献。在添加所需要设置的转化变量的代码之前，需要在 GrowingIO 产品的`自定义事件和变量`管理页面配置转化级变量。

接口定义：

```text
gio('setEvar', properties: object)
```

参数说明：

| 参数名称 | 参数类型 | 是否必须 | 说明 |
| --- | --- |
| properties | object | 是 | 转化级变量，转化信息 |

示例：

```text
// 假设初始化后把 gio 对象放在 App 的 globalData 里面
getApp().globalData.gio('setEvar', { 
  campaign: '活动A'
});
```



