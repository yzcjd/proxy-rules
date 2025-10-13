##### 备注 1：测速链接不同只是为了方便自动选择，测试结果延迟高低对节点无影响。
##### 备注 2：Clash 规则其他软件也可套用，包括 singbox，已标出例外。暂未给其他软件写规则，对应的分流应该会自动适配。（singbox 偶尔不兼容）

### 直接使用
#### https://fatsheep.yzcjd.workers.dev

### 其他订阅转换套用
##### 「远程配置」填入规则，可合并多个鸡场订阅
#### Clashmeta 订阅转换： https://sub.v1.mk
#### Clash 订阅转换：https://sub.dler.io
.

#### 使用建议：
##### 不知道怎么用 => 导入第一个规则 clash.ini 试试
##### 日常浏览 => V2fly 规则（防延迟劫持）
##### 同时看多个视频网站 =>  负载均衡规则（load）
##### Telegram 重度用户 => TG 优化规则 三选一，常看中文频道选 tg 规则，常看欧美频道选 tg2 或 tg3（tg3 需有港新澳台马印以外线路）；
##### 推荐尝试 GEOIP 规则自动分流
.

.

### 白名单规则【clash.ini】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.ini
.
##### 1. 测速链接使用“ http://www.gstatic.com/generate_204 ”（clash 默认）
##### 2. 中国域名、ip 走直连，其他走代理。
##### 3. 多地区自动选择，TG 可选 All、HK、SG 分组内延迟最低。（已移除）
##### surfboard 可用
.

.

### 轻量白名单规则【lite】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.lite.ini
.
##### 港日新+手动
##### surfboard 可用
.

.

### 全局规则【global】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.global.ini
.
##### 1. 全局规则 + 地区分组 。解决全局模式下不能自动选择的问题。
##### 2. 只有全局，内网直连。没加规则模式。
##### 3. 如果你某部手机只访问外网，建议关闭订阅自动更新（订阅转换站有时拉取规则会出错）
##### surfboard 可用
.

.

### TG 优化规则1【tg】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.tg.ini
.
####  中文频道规则（新加坡服务器）
##### TG 延迟测速“ http://91.108.56.200 ”，多地区自动选择；
##### 该测试不准，仅参考。测试超时 ≠ 连不上 Telegram ，有延迟 ≠ 可以用。
##### surfboard 可用
.

.

### TG 优化规则2【tg2】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.tg2.ini
#### 英文频道规则（英国服务器）
##### 1. TG 延迟测速“ http://149.154.164.250 ”。多地区自动选择；
##### 2. 延迟结果为 Telegram 英文频道延迟。默认使用选择的地区上网（不要看延迟），受影响：英文频道、Telegraph、TG预览。
##### 3. 如果你要优化 TG 中文频道访问，推荐使用香港自动或者新加坡自动（非最优），不影响 TG2 自动选择 。
##### 4. 该测试不准，测试超时 ≠ 连不上 Telegram ，有延迟 ≠ 可以用。
##### surfboard 可用
.

.

### TG 优化规则3【tg3】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.tg3.ini
##### 1. 综合中文频道和英文频道规则，适合综合浏览。
##### 2. 港新马台澳印测试 “ http://91.108.56.200 ”，其它测试 “ http://149.154.164.250 ”。常用地区自动选择；
##### 3. 屏蔽常见广告，尽量做到无误杀，具体查看 https://raw.githubusercontent.com/yzcjd/website-rules/1/REJECT
##### 4. surfboard 用这规则偶尔报错。
.

.

### 分地区负载均衡【load】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.load.ini
.
#### 特点
##### 测速链接同 Clash 默认。负载均衡模式下延迟无意义，保证你节点带宽足够就行。
##### 每个域名用不同的节点，举例：可以实现 TG 视频、YouTube、TED 同时播放网速不冲突。
##### 需确定机场的节点为同一地区，否则可能遇到 Google 人机验证。
测试网页 [ip.sb](https://ip.sb/) ，①连上节点打开网站 **OR** ②复制 域名（xx.xx.com）/ ip 在 ping0.cc / ip.sb 搜索。
##### surfboard 可用
.

.

### V2fly 规则【v2fly】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.v2fly.ini
.
#### 特点
##### Sagernet 默认测速链接（https），真实延迟，避免机场劫持测速结果 ；
##### 该规则 surfboard 不可套用（内含 https 测速链接）。
.

.

### 自用规则 【cool】
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/clash.cool.ini
.
#### 特点
##### Google 服务可选地区（已注释），GitHub、x、netflix、openai、imgur等常用网站优化，全自动无需手动选。
##### 浏览网页排除送中节点，看视频排除 IEPL 专线节点。如果全是专线（名字全部带IEPL/IPLC，必须手动改名字才能用），你的线路如果送中，名字添加 sz，浏览网页将不会选中他。
##### 该规则 surfboard 不可套用（内含 https 测速链接）。
##### PS：这仅是本人自用规则。推荐尝试 GEOIP 规则自动分流，手动添加的规则永远有优化空间。
.
———————————————————————————————————————

.
### Surfboard 规则（白名单玩具版）
https://raw.githubusercontent.com/yzcjd/proxy-rules/main/surfboard.ini

### 特点
##### 1. 测速链接使用 “ http://cp.cloudflare.com ” 
##### 2. 多地区自动选择，TG 可选 HK、SG 分组；
##### 3. 当前只是套用 Clash 模板，先用着，以后再写。（冲浪板支持协议少，可能不写了）
##### 4. 该规则 Clash 也能用，emmm 大可不必。
.

### ShadowRocket 规则（白名单玩具版）
##### 配置 => 右上角"+" => 粘贴链接： https://raw.githubusercontent.com/yzcjd/proxy-rules/main/shadowrocket.ini => 选择配置使用。
.

#### 部分规则已归档，点击 file 文件夹查看。路径不同。
.
#### 下一阶段：clash：专线组（特定网站走专线）、锁定某个网站/服务的定位
#### 下下阶段：完善 Surfboard 规则
待更新咕咕咕
