## 订阅转换：[dler](https://sub.dler.io/)， 填入远端配置。


### ① clash 规则（白名单）：
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.ini

### ② clash 轻量规则（白名单）：
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.lite.ini

### 通用特点
#### 1. 测速链接使用“ https://github.com ”，测速间隔 30 秒，相差 150 ms 才切换节点。
#### 2. 节点根据名字分类地区，目前只有自动选择。TG 可选 All、HK、SG 分组内延迟最低；
#### 3. 统一节点名称为国家代码，如美国节点名改成 US、沪日 IEPL 改成 JP IEPL，“游戏x5 韩国”改成“KR game”
#### 4. 
##### ①号规则：只有自动选择，分组为 港日新韩美+全部；
##### ②号规则：包含手动选择，港日新支持自动选择（其他：手动选择分组），适合自建使用。
——————————————————————————————————————————————————————————————————
### ③ Surfboard 规则（玩具版）
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/surfboard.ini


### 特点
#### 1. 测速链接使用 “ http://cp.cloudflare.com ) ” ，测速间隔 30 秒，相差 150 ms 才切换节点。
#### 2. 改名、自动选择，TG 可选分组；
#### 3. 现在只是套用 Clash 模板，先用着，以后再更新。

.

#### 下一阶段：clash：专线组（特定网站走专线）、分地区负载均衡、IP 锁定地区
#### 下下阶段：完善 Surfboard 规则
待更新咕咕咕
