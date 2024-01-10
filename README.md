### Clash 订阅转换：[墙洞转换](https://sub.dler.io/) 
### Clashmeta 订阅转换： [肥羊转换](sub.v1.mk)

.

## ----------  「远程配置」填入规则，可合并多个鸡场订阅   ----------

.
##### 备注 1：测速链接不同只是为了方便自动选择，测试结果延迟高低对节点无影响。
##### 备注 2：Clash 规则其他软件也可套用，已标出例外。暂未给其他软件写规则，其他软件的分流应该是自动适配。
##### 推荐：
##### Telegram 重度用户 => TG 优化规则 三选一；
##### 日常浏览 => V2fly 规则、TG 选择 HK 或 SG
.

.

### ① 白名单规则【clash.ini】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.ini

### 特点
##### 1. 测速链接使用“ http://www.gstatic.com/generate_204 ”（clash 默认）
##### 2. 中国域名、ip 走直连，其他走代理。
##### 3. 多地区自动选择，TG 可选 All、HK、SG 分组内延迟最低。
##### surfboard 可用
.

.

### ② 轻量白名单规则【lite】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.lite.ini
.
#### 特点
##### 港日新+手动
##### surfboard 可用
.

.

### ③ 全局规则【global】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.global.ini
.
#### 特点
##### 1. 全局规则 + 地区分组
##### surfboard 可用
.

.

### TG 优化规则1【tg】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.tg.ini
.
#### 中文频道规则（新加坡服务器）
##### 1. TG 延迟测速“ http://91.108.56.200 ”，多地区自动选择；
##### 2. 有 Clash 延迟测速，方便对比。
##### 3. 该测试不准，仅参考。测试超时 ≠ 连不上 Telegram ，有延迟 ≠ 可以用。
##### surfboard 可用
.

.

### TG 优化规则2【tg2】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.tg2.ini
#### 英文频道规则（英国服务器）
##### 1. TG 延迟测速“ http://149.154.164.250 ”。多地区自动选择；
##### 2. 延迟结果为 Telegram 英文频道延迟。默认使用选择的地区上网（不要看延迟），受影响：英文频道、Telegraph、TG预览。
##### 3. 如果你要优化 TG1 访问，推荐使用香港自动或者新加坡自动（非最优），不影响 TG2 自动选择 。
##### 4. 有 Clash 延迟测速，方便对比。
##### 5. 该测试不准，测试超时 ≠ 连不上 Telegram ，有延迟 ≠ 可以用。
##### surfboard 可用
.

.

### TG 优化规则3【tg3】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.tg3.ini
##### 1. 综合中文频道和英文频道规则，以及德国服务器规则，适合综合浏览。
#####    如果你只有热门地区，不推荐使用此规则。至少需要有新加坡（暂时移除，因为必定选中新加坡），具体国家点开规则查看。
##### 2. 没加对应网站的手动选择。
##### 3. 测速链接“ https://api.v2fly.org/checkConnection.svgz ”。多地区自动选择；
##### 4. Surfboard 不可套用。
.
##### 备注：均衡的节点，测试规则 tg、tg2 都是 400ms，如：越南、泰国、哥斯达黎加。
##### surfboard 可用
.

.

### 分地区负载均衡【load】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.load.ini
.
#### 特点
##### 测速链接同 Clash 默认。负载均衡模式下延迟无意义，保证你节点带宽足够就行。
##### 每个域名用不同的节点，举例：可以实现 TG 视频、YouTube、TED 同时播放网速不冲突。
##### 请确定机场的节点为同一地区，否则会有人机验证。
测试网址 [ip.sb](https://ip.sb/) ，①连上节点打开网站 **OR** ②复制 ip 搜索。
##### surfboard 可用
.

.

### Google优化【google】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.google.ini
.
#### 特点
##### 测试 本地 => 节点 => Google 美国服务器，能看出节点的国际互联情况；
##### 参考值：300ms ；合格值：600ms 我猜的。
##### 该规则 surfboard 不可套用（内含 https 测速链接）。
.

.

### V2fly 规则【v2fly】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.v2fly.ini
.
#### 特点
##### Sagernet 默认测速链接，也许能测试节点是否送中；
##### 该规则 surfboard 不可套用（内含 https 测速链接）。
.

.

### 自用规则 【cool】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.cool.ini
.
#### 特点
##### Google 可选地区，Telegram、GitHub 等常用网站优化。
##### 测试中，随时修改。不一定适合你，我没有固定地区需求，甚至可能取消地区分组。
##### 该规则 surfboard 不可套用（内含 https 测速链接）。
.
———————————————————————————————————————

.
### Surfboard 规则（玩具版）
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/surfboard.ini

### 特点
##### 1. 测速链接使用 “ http://cp.cloudflare.com ” 
##### 2. 多地区自动选择，TG 可选分组；
##### 3. 当前只是套用 Clash 模板，先用着，以后再更新。Clash 也能用，延迟测试数值偏低。
.

.

#### 部分规则已归档，点击file文件夹查看
.
#### 下一阶段：clash：专线组（特定网站走专线）、分地区负载均衡、IP 锁定地区
#### 下下阶段：完善 Surfboard 规则
待更新咕咕咕
