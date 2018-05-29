# SDK 采集数据和逻辑

GrowingIO 的小程序 SDK 支持两种采集数据：无埋点自动采集事件和自定义事件。无埋点采集事件可以让你方便地获取数据概况，灵活定义指标，快速搭建指标体系。自定义事件则可以让你完全控制数据指标，拥有更大的自主权，获取更多的数据探索和洞察。结合无埋点事件和自定义事件来搭建一套完善的指标体系，可以为后续的分析优化提供坚实的基础。

作为用户行为数据分析工具，用户信息的完善会给后续的分析带来很大的帮助。下面是专门针对用户的三个接口。

#### 绑定微信用户ID

当用户在你的小程序上登陆获取到 openid 后，可以用过 `identify` 接口绑定微信用户ID，后续在 GrowingIO 中获取更准确的微信访问用户量。示例代码如下，

```javascript
wx.request({ 
  url: 'https://YOUR_HOST_NAME/wechat/code2key',
  method: 'GET',
  data: { code: res.code }
  success: res => 
    var openid = res.data.openid;
    var unionid = res.data.unionid;
    ...
    gio('identify', res.data.openid, res.data.unionid)
})
```

如果你希望直接用 openid 来替换 GrowingIO 自行设置的用户标识符，请在初始化的时候指定 forceLogin 参数为 true。详见

{% page-ref page="../sdk-integration.md" %}

#### 设置微信用户信息

当用户在你的小程序上绑定微信信息后，可以通过 `setVisitor` 接口设置微信用户信息，后续在 GrowingIO 中分析这个数据。示例代码如下，

```javascript
wx.getUserInfo({ 
  success: res => 
    ...
    gio('setVisitor', res.userInfo);
})
```

微信信息包含微信昵称、微信头像、性别、微信所填国家、微信所填省份、微信所填城市。

#### 设置注册用户ID

当用户在你的小程序上注册以后，你的产品应用服务端会在用户数据库里添加一条记录并且分配一个 ID，可以通过 setUserId 接口设置注册用户ID，后续在 GrowingIO 中分析登录用户这个数据。示例代码如下，

```javascript
gio('setUserId', YOUR_USER_ID); 
```



