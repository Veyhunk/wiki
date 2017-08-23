此功能最低要求 1.0.3 版本，如低于此版本，[请升级](http://ksria.com/simpread/) 到最新版本。
***

### 含义：
此功能是将由简悦优化后的 `阅读模式` 的页面发送到 Kindle 上，而非（转换前）原文。

### 第三方服务：
此功能使用了第三方服务 http://fivefilters.org/kindle-it ，所以请确保你的网络可以访问它。

### 配置：
> 需要将 http://fivefilters.org/kindle-it 对应的信箱 `kindle@fivefilters.org` 加入到 Kindle 的白名单中。

- 使用你的账户登陆并打开 https://www.amazon.cn/mn/dcw/myx.html#/home/settings/payment
- 找到 `已认可的发件人电子邮箱列表` 节，并将 `kindle@fivefilters.org` 加入信任列表，如图：
  ![Imgur](http://i.imgur.com/m406zSC.png)

### 使用：
> 由于转码使用了简悦自己的后台服务，所以请确保可以访问 https://simpread.herokuapp.com

- 打开 `阅读模式` 后，通过控制栏进行发送（下图），当转码成功后，会自动打开 fivefilters.org 发送页面，如 [测试页面](http://fivefilters.org/kindle-it/send.php?url=https://simpread.herokuapp.com/view/demo.htm)
  