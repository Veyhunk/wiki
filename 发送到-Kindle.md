此功能最低要求 1.0.3 版本，如低于此版本，[请升级](http://ksria.com/simpread/) 到最新版本。
***

目录
---
- [入口](https://github.com/Kenshin/simpread/wiki/%E8%87%AA%E5%AE%9A%E4%B9%89%E4%B8%BB%E9%A2%98#%E5%85%A5%E5%8F%A3)
- [界面说明](https://github.com/Kenshin/simpread/wiki/%E8%87%AA%E5%AE%9A%E4%B9%89%E4%B8%BB%E9%A2%98#%E7%95%8C%E9%9D%A2%E8%AF%B4%E6%98%8E)
- [优先级](https://github.com/Kenshin/simpread/wiki/%E8%87%AA%E5%AE%9A%E4%B9%89%E4%B8%BB%E9%A2%98#%E4%BC%98%E5%85%88%E7%BA%A7)
- [无法更新阅读模式的 「主题、字体样式、字体大小、版面布局」](https://github.com/Kenshin/simpread/wiki/%E8%87%AA%E5%AE%9A%E4%B9%89%E4%B8%BB%E9%A2%98#%E6%97%A0%E6%B3%95%E6%9B%B4%E6%96%B0%E9%98%85%E8%AF%BB%E6%A8%A1%E5%BC%8F%E7%9A%84-%E4%B8%BB%E9%A2%98%E5%AD%97%E4%BD%93%E6%A0%B7%E5%BC%8F%E5%AD%97%E4%BD%93%E5%A4%A7%E5%B0%8F%E7%89%88%E9%9D%A2%E5%B8%83%E5%B1%80)

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
  ![Imgur](http://i.imgur.com/v49dYXs.png)

### 注意：
- 生成后的页面，如 `https://simpread.herokuapp.com/view/20170823xxxxxx.html` 并不会长久存在，超时后会自动删除。