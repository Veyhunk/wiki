目录
---
- [离线安装](https://github.com/Kenshin/simpread/wiki/入门指南（-操作指引-）#离线安装)
- [排除列表](https://github.com/Kenshin/simpread/wiki/入门指南（-操作指引-）#排除列表)
- [快捷键](https://github.com/Kenshin/simpread/wiki/入门指南（-操作指引-）#快捷键)

- [阅读模式无法正常](https://github.com/Kenshin/simpread/wiki/%E5%85%A5%E9%97%A8%E6%8C%87%E5%8D%97%EF%BC%88-%E6%93%8D%E4%BD%9C%E6%8C%87%E5%BC%95-%EF%BC%89#%E6%9F%90%E4%BA%9B%E7%AB%99%E7%82%B9%E5%B7%B2%E7%BB%8F%E9%80%82%E9%85%8D%E4%BA%86%E9%98%85%E8%AF%BB%E6%A8%A1%E5%BC%8F%E4%BD%86%E6%97%A0%E6%B3%95%E6%AD%A3%E5%B8%B8%E6%98%BE%E7%A4%BA%E7%9A%84%E9%97%AE%E9%A2%98)
- [测试版通道](https://github.com/Kenshin/simpread/wiki/%E5%85%A5%E9%97%A8%E6%8C%87%E5%8D%97%EF%BC%88-%E6%93%8D%E4%BD%9C%E6%8C%87%E5%BC%95-%EF%BC%89#%E6%B5%8B%E8%AF%95%E7%89%88%E9%80%9A%E9%81%93)
- [自定义样式](https://github.com/Kenshin/simpread/wiki/FAQ#%E8%87%AA%E5%AE%9A%E4%B9%89%E6%A0%B7%E5%BC%8F)
- [授权服务](https://github.com/Kenshin/simpread/wiki/FAQ#%E6%8E%88%E6%9D%83%E6%9C%8D%E5%8A%A1)
- [发送到 Kindle](https://github.com/Kenshin/simpread/wiki/FAQ#%E5%8F%91%E9%80%81%E5%88%B0-kindle)

***

离线安装
---

进入 http://ksria.com/simpread 选择 `离线下线`
![Imgur](http://i.imgur.com/ocmtcSpl.png)

- Widows 系统
  - 将下载的 `simpread.crx` 拖拽到  `chrome://extensions/` 即可。

- MAC OS 系统
  > 参考 [将非官方扩展程序加入 Chrome 的白名单](https://hencolle.com/2016/10/16/baidu_exporter/)
  - 下载 https://gist.github.com/Explorare/be3dd598289252698cd37bca04abd0fe#file-com-google-chrome-mobileconfig
  - 打开添加 `<string>dniikipdjeghiehnmendnfiinmhadidp</string>` 并保存
    ![Imgur](http://i.imgur.com/QozEOJGl.png)
  - 双击此文件，按照弹出的提示点击 `继续` → `安装（输入电脑密码）`
  - 重启浏览器即可！

排除列表
---

> 当选中 `如果当前页面适配阅读模式，是否自动进入阅读模式？` 会启动此功能，加入到列表中的 URL 将不会自动进入阅读模式。（ 但不影响手动操作 ）
---
![Imgur](http://i.imgur.com/dyROEBi.png) → 右键 → 选项 → 高级设定 → 排除列表` ，如图：
![Imgur](http://i.imgur.com/CdoZOkUl.png)

添加规则：
- 支持 URL 如： http://www.jianshu.com/p/2917e4e0169d
- 支持 [minimatch](https://github.com/isaacs/minimatch) 方案的 URL，如：`http://*.cnbeta.com/articles/*/*.htm`
- 支持 [站点编辑器 的 name](https://github.com/Kenshin/simpread/wiki/站点编辑器#对应字段)，如：  
![Imgur](http://i.imgur.com/IFc5kAEl.png) 

快捷键
---
> 简悦支持快捷键，但是由于与 cVim 等扩展有些冲突，所以并没有指出。

- 全局支持 `ESC` 退出；  
  包括：`聚焦模式` `阅读模式` 以及 它们的 `设定对话框`；

- 可编辑的快捷键：
   - `聚焦模式`（默认为 `A S` ) 
   - `阅读模式` （默认为 `双击 A` ) 

- 不可编辑的快捷键：
  > 只限 `阅读模式`，包括：`字体类型` `字体大小` `版面布局`，如图：  
  
  ![Imgur](http://i.imgur.com/KgIhnoVl.png)  
  ![Imgur](http://i.imgur.com/Y7vCUFll.png)  
  ![Imgur](http://i.imgur.com/ebbvkIDl.png) 

某些站点已经适配了阅读模式，但无法正常显示的问题
---

[站点编辑器](https://github.com/Kenshin/simpread/wiki/站点编辑器) 使用了 URL 适配规则，加入相同规则的 URL 对应页面的结构如果不相同，如：  

> http://www.jianshu.com/p/2917e4e0169d  
> http://www.jianshu.com/p/2917e4e0169de

就会出现如下界面：  
![Imgur](http://i.imgur.com/jckXO4yl.png)

目前这种情况的解决办法是将此 URL 加入到 [排除列表](https://github.com/Kenshin/simpread/wiki/入门指南（-操作指引-）#排除列表) 或者 [报告给我](https://github.com/Kenshin/simpread/issues/new)。

测试版通道
---
测试版下载说明，请移步 [这里](https://github.com/Kenshin/simpread/wiki/%E6%B5%8B%E8%AF%95%E7%89%88)

自定义样式
---
关于 自定义样式 的FAQ，请 [访问这里](https://github.com/Kenshin/simpread/wiki/%E8%87%AA%E5%AE%9A%E4%B9%89%E6%A0%B7%E5%BC%8F)

授权服务
---
关于 授权服务 的FAQ，请 [访问这里](https://github.com/Kenshin/simpread/wiki/%E6%8E%88%E6%9D%83%E6%9C%8D%E5%8A%A1)

发送到 Kindle
---
关于 发送到 Kindle 的FAQ，请 [访问这里](https://github.com/Kenshin/simpread/wiki/%E5%8F%91%E9%80%81%E5%88%B0-Kindle)