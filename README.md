## 概述

用于在 Heroku 上免费搭建加速节点从而加速游戏

**Heroku 为我们提供了免费的容器服务，我们不应该滥用它，所以本项目不宜做为长期加速使用。**

**可以部署两个以上的应用，实现 [负载均衡](https://toutyrater.github.io/routing/balance2.html)，避免长时间大流量连接某一应用而被 Heroku 判定为滥用。**

**Heroku 的网络并不稳定，部署前请三思。**

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https://github.com/lpmon1/v2ray-heroku)

## ENV 设定

### UUID

`UUID` > `一个 UUID，供用户连接时验证身份使用`。

## 注意

WebSocket 路径为 `/`。

`alterId` 为 `64`。

V2Ray 将在部署时自动安装最新版本。

**出于安全考量，除非使用 CDN，否则请不要使用自定义域名，而使用 Heroku 分配的二级域名，以实现 V2Ray Websocket + TLS。**
