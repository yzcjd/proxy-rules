### Clash 订阅转换：[墙洞转换](https://sub.dler.io/) 
### Clashmeta 订阅转换： [肥羊转换](sub.v1.mk)

，

## ----------  「远程配置」填入规则，可合并多个鸡场订阅   ----------

.

##### 备注 1：测速链接不同只是为了方便自动选择，测试结果延迟高低对节点无影响。
##### 备注 2：Clash 规则其他软件也可套用，已标出例外。暂未给其他软件写规则，分流不细致。
##### 推荐：如果看电报比较多，推荐 TG 优化； 日常使用浏览，推荐 cool 订阅并固定地区。

，

，

### ① clash 规则（白名单）【clash.ini】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.ini

### 特点
##### 1. 测速链接使用“ http://www.gstatic.com/generate_204 ”（clash 默认），测速间隔 30 秒，低延迟地区相差 50 ms 切换节点、高延迟地区相差 70ms、100ms 切换节点；
##### 2. 多地区自动选择；
##### 3. TG 可选 All、HK、SG 分组内延迟最低。

，

### ② clash 轻量规则（白名单）【lite】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.lite.ini
.
#### 特点
##### 1. 港日新+手动；
##### 2. 测速链接使用“ https://www.google.com ”，真实谷歌延迟。
##### 3. 该规则 surfboard 不可套用（因为是 https 链接）。
.

### ③ TG 优化规则1【tg】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.tg.ini
.
#### 特点
##### 1. TG 延迟测速“ http://91.108.56.200 ”新加坡 DC5 服务器，多地区自动选择；
ps：+86 手机号注册的 TG 使用 DC5 新加坡服务器。如果你不是 DC5，自行更改链接（查看 Clash 连接日志）。
##### 2. 有 Clash 延迟测速，方便对比。
##### 3. 该测试不准，图一乐。测试超时 ≠ 连不上 Telegram ，有延迟 ≠ 可以用。
##### 4. 以免误用 IEPL 刷 TG，默认使用选择的地区连接 Telegram ，推荐切换成所有节点（TG Ping）。
 clash TG 优化规则1【tg】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.tg.ini

.

.
### ③ TG 优化规则2【tg2】
#### 特点
##### 1. TG 延迟测速“ http://149.154.164.250 ”，英国伦敦服务器，多地区自动选择；
ps：如果你不是 DC5 ，可能连接的服务器不同。可查看 Clash 连接日志更换测速链接。
##### 2. 有 Clash 延迟测速，方便对比。
##### 3. 该测试不准，测试超时 ≠ 连不上 Telegram
##### 4. 以免误用 IEPL 刷 TG，默认使用选择的地区连接 Telegram，推荐切换成所有节点（TG Ping）。
.

### ④ clash Google优化 【cool】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.cool.ini
.
#### 特点
##### 测试 本地 =>> 节点 =>> Google 美国服务器，能看出节点的国际互联情况；
##### 参考值：300ms ；合格值：600ms 我猜的。
##### 该规则 surfboard 不可套用（内含 https 测速链接）。
.

### ⑤ clash 大杂烩优化 【test】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.cool.ini
.
#### 特点
##### Telegram、GitHub 等常用网站优化。
##### 该规则 surfboard 不可套用（内含 https 测速链接）。
.

### ⑥ clash Fastly 优化 【fastly】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.cool.ini
.
#### 特点
##### 测速链接使用 “ https://imgur.com/ ” ，测试本地网络 => 节点 => 美国 Fastly 节点。
##### ps：各网站服务器遍布全球，可以看出节点的国际互联情况。
##### 该规则 surfboard 不可套用（因为是 https 链接）。
.

### ⑥ clash 分地区负载均衡【load】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.load.ini
.
#### 特点
##### 测速链接同 Clash 默认。
##### 每个域名用不同的节点，举例：可以实现 TG 视频、YouTube、TED 同时播放网速不冲突。
##### 请确定机场的节点为同一地区，否则会有人机验证。
测试网址 [ip.sb](https://ip.sb/) ，①连上节点打开网站 **OR** ②复制 ip 搜索。
##### 该规则 surfboard 不可套用（因为是 https 链接）。

.
———————————————————————————————————————

.
### Surfboard 规则（玩具版）
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/surfboard.ini

### 特点
##### 1. 测速链接使用 “ http://cp.cloudflare.com ” ，测速间隔 30 秒，相差 150 ms 才切换节点。
##### 2. 多地区自动选择，TG 可选分组；
##### 3. 当前只是套用 Clash 模板，先用着，以后再更新。Clash 也能用，延迟测试数值较低。

.

#### 下一阶段：clash：专线组（特定网站走专线）、分地区负载均衡、IP 锁定地区
#### 下下阶段：完善 Surfboard 规则
待更新咕咕咕
