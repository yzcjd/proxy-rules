## 订阅转换：[dler](https://sub.dler.io/)， 填入远端配置。

.

### ① clash 规则（白名单）：
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.ini

### 特点
##### 1. 测速链接使用“ https://api.v2fly.org/checkConnection.svgz ”，测速间隔 30 秒，相差 150 ms 才切换节点；
##### 2. 多地区自动选择；
##### 3. TG 可选 All、HK、SG 分组内延迟最低。

.

### ② clash 轻量规则（白名单）：
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.lite.ini
.
#### 特点
##### 1. 港日新+手动；
##### 2. 还没想到，但是前面写了个1

.

### ③ clash TG 优化规则：
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.tg.ini
.
#### 特点
##### 1. TG 延迟测速“ http://91.108.56.200 ”，多地区自动选择；
ps：+86 手机号注册的 TG 使用 DC5 新加坡服务器。如果你不是 DC5，自行更改链接（查看 Clash 连接日志）。
##### 2. 有 Clash 延迟测速，方便对比。

.

### ④ clash 薯条机场节点名简化规则：
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.cnix.ini
.
#### 特点
##### 1. TG 优化规则修改，仅针对“薯条CNIX”机场简化节点名；
##### 2. 还没想到，但是前面写了个1

.
———————————————————————————————————————

.
### ① Surfboard 规则（玩具版）
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/surfboard.ini

### 特点
##### 1. 测速链接使用 “ http://cp.cloudflare.com ” ，测速间隔 30 秒，相差 150 ms 才切换节点。
##### 2. 多地区自动选择，TG 可选分组；
##### 3. 当前只是套用 Clash 模板，先用着，以后再更新。Clash也能用，延迟测试数值较低。

.

#### 下一阶段：clash：专线组（特定网站走专线）、分地区负载均衡、IP 锁定地区
#### 下下阶段：完善 Surfboard 规则
待更新咕咕咕
