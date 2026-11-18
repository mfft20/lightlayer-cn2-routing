# lightlayer cn2 购买指南：哪条线路才走 CN2？$24.99/年 的套餐带宽够不够？（附测试 IP 与全套餐价格对照）

LightLayer 的 CN2 只出现在 Premium 线路上，Standard 和 Global 都不走。官方在 2024 年 7 月发布的活动页把洛杉矶的三条线写得很清楚：Premium 是 CN2 + Mainland BGP + International BGP，Standard 是 Mainland BGP + International BGP，Global 只有 International BGP。台湾和马尼拉各提供 Premium 与 Global 两条线路，没有 Standard。

这条 CN2 线路最便宜的入口是年付 $24.99，配置为 1 核 CPU、1G 内存、50G 硬盘。这个价位的带宽只有 20M 不限流量，或者 30M 配 1TB 月流量。前排测评里常见的“100Mbps 不限量”说的是 Global 线，两者并不是一回事，而这一点恰恰是下单前最该弄清楚的地方。

下面把三条线的区别、全套餐价格、官方测试 IP 和真实成本逐一核对一遍。

## 选购速览

> **只跑小站、做开发测试、用户不在大陆**：Startup 的 Global 线，$4/月，100Mbps 不限量，不需要为 CN2 付钱。
>
> **明确需要中国大陆方向低延迟**：洛杉矶 Premium，年付 $49.99；预算卡得紧就选 1C/1G 年付 $24.99 的 Premium 档，但要知道带宽只有 20M 或 30M。
>
> **用户在台湾、东南亚**：台湾或马尼拉的 Premium，年付 $24.99。
>
> 👉 [查看洛杉矶 Premium 的套餐与当前价格](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74)

## 全套餐价格对照

官方目前能查到的一手价格表，是 2024 年 7 月 10 日发布的夏季活动页。页面标题写着 “Only $24.99 per year”，覆盖洛杉矶、台湾、马尼拉三个机房，配置统一为 1 核、1G 内存、50G 硬盘，活动结束日期写的是 8 月 31 日，并注明 renew at the same price。

| 线路 | 端口 / 流量 | 机房 | 年付价 | 下单 |
| --- | --- | --- | --- | --- |
| Premium（CN2） | 20M / 不限流量 | 洛杉矶 | $24.99 | [选这档](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74) |
| Premium（CN2） | 30M / 1TB 每月 | 洛杉矶 | $24.99 | [选这档](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74) |
| Standard | 50M / 不限流量 | 洛杉矶 | $24.99 | [选这档](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74) |
| Standard | 100M / 1TB 每月 | 洛杉矶 | $24.99 | [选这档](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74) |
| Standard | 1G / 1TB 每月 | 洛杉矶 | $83.99 | [选这档](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74) |
| Global | 100M / 不限流量 | 洛杉矶 | $24.99 | [选这档](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74) |
| Global | 200M / 1TB 每月 | 洛杉矶 | $24.99 | [选这档](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74) |
| Global | 1G / 1TB 每月 | 洛杉矶 | $41.99 | [选这档](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74) |

台湾和马尼拉同样参与这次活动，起价也是 $24.99/年，但只有 Premium 和 Global 两条线可选，没有 Standard。想要这两个机房的话从这里进：

| 机房 | 可选线路 | 年付价 | 下单 |
| --- | --- | --- | --- |
| 马尼拉 | Premium / Global | $24.99 | [查看马尼拉套餐](https://account.lightlayer.net/index.php?/cart/manila/&affid=74) |
| 台湾 | Premium / Global | $24.99 | [查看台湾套餐](https://account.lightlayer.net/index.php?/cart/taiwan/&affid=74) |

第三方测评整理的月付档位是另一套口径，适合不想一次性付一年的人：

| 档位 | 配置 | 线路 | 起价 | 下单 |
| --- | --- | --- | --- | --- |
| Startup | 1 核 / 1GB / 50GB SSD / 100Mbps 不限 | Global | $4.00/月 | [查看月付档](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74) |
| Pay As You Go | 2 核起 / 2GB 起 / 存储可调 / 200Mbps+ | Standard | $5.60/月起 | [自选配置](https://account.lightlayer.net/index.php?/cart/specialoffer/&affid=74) |
| Mid-Tier | 4 核 / 4GB / 80GB SSD / 200Mbps 不限 | Standard 或 Premium | 约 $11–18/月 | [查看中配](https://account.lightlayer.net/index.php?/cart/specialoffer/&affid=74) |
| Business | 32 核 / 32GB / 存储可调 / 200Mbps 不限 | Premium | $53.60/月 | [查看高配](https://account.lightlayer.net/index.php?/cart/specialoffer/&affid=74) |

这里要说明白：不同来源的配置口径不一致。官方活动页写 50G 硬盘，第三方 2026 年 3 月的一份整理写 20GB SSD；带宽上，有的来源写 100Mbps 不限量，有的写 1Gbps 配 1TB 流量。这些差异来自不同时间点的不同促销档，没法合并成一个结论。下单时以结账页显示的配置和价格为准。

另外，洛杉矶 Premium 的年付价在第三方表里是 $49.99，Global 是 $29.99，Standard 是 $39.99。同样 1 核 1G 的硬件，三条线差出 $20，差的就是网络路径。

## LightLayer 的 CN2 到底是哪条线

三条线的官方定义没有歧义：

- **Premium**：CN2 + Mainland BGP + International BGP，官方原话是大陆用户“延迟最低、线路最稳”。
- **Standard**：Mainland BGP + International BGP，走大陆方向但不含 CN2。
- **Global**：International BGP，面向大陆以外的海外用户和美国本地用户。

台湾和马尼拉只提供 Premium 和 Global。

官方只写了“CN2”，没写是 GIA 还是 GT。第三方测评在 2026 年的文章里普遍写成“CN2 GIA + 中国移动 CMIN2”。官方的措辞更保守，第三方的说法更具体但不是官方口径，两者都可以参考，真要确认还得看回程。

有一份第三方整理的 2026 年资料称 Standard 线路“在某些路由上接 CN2”，这和官方定义直接冲突。官方写的是 Standard = Mainland BGP + International BGP，没有 CN2。以官方为准，Standard 不含 CN2。

官方 2024 年的活动页只列了洛杉矶、台湾、马尼拉三地。第三方在 2026 年的测评里还提到圣何塞有 Premium 优化线路、香港和东京有 CN2 档位。这些没有官方页面佐证，只能当线索：如果你对圣何塞感兴趣，去购物车页面自己确认一遍再下单。

## 用官方测试 IP 自己验证线路

官方在活动页公布了六个测试 IP，这是整篇资料里最实用的部分。买之前花十分钟自己测，比看任何测评都准。

| 机房 | 线路 | 测试 IP |
| --- | --- | --- |
| 洛杉矶 | Premium | 38.61.2.254 |
| 洛杉矶 | Standard | 38.61.5.254 |
| 洛杉矶 | Global | 38.61.7.254 |
| 台湾 | Premium | 46.8.124.242 |
| 台湾 | Global | 46.8.126.64 |
| 马尼拉 | Premium | 154.39.138.254 |
| 马尼拉 | Global | 154.39.140.254 |

这组 IP 来自 2024 年 7 月的活动页，可能已经变动，测不通就换下一个机房。

怎么测：

1. **ping 连续跑 100 个包**，看丢包率和抖动。偶尔一次 ping 通说明不了问题，晚高峰的稳定性才是关键。
2. **traceroute 或 mtr 看回程路径**。把 Premium 和 Global 两个 IP 的路径并排对比，Premium 的节点数量和跳转方式应该和 Global 明显不同。路径一样就说明你买错了档。
3. **分时段测**。晚 8 点到 11 点一次，凌晨一次。两个时段差距大，说明这条线在高峰期会拥塞。
4. **三家运营商分别测**。电信、联通、移动走的路由不一样，你用户用什么宽带就测什么。

同一个机房的 Premium 和 Global 对比着测，两条线之间的差值，就是你多付那 $20 一年买到的东西。值不值，测完自己判断。

👉 [按机房对比当前套餐](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74)

## $24.99 一年，实际买到了什么

$24.99 除以 12 个月，约等于每月 $2.08。同样的 1 核 1G 配置，月付 Global 档是 $4/月，一年 $48。年付省下的钱是实打实的。

但便宜的那档 CN2 有代价。$24.99 的 Premium 只有两种带宽规格：20M 不限流量，或者 30M 配 1TB 月流量。两个价格一样，选哪个取决于你的用法：流量小但要求持续在线，选 20M 不限量；平时空闲、偶尔跑满，选 30M 带 1TB。想跑满 100Mbps 的 CN2，这个价位给不了。

洛杉矶同期还上线了 1Gbps 端口的产品，但那是另一个价位。官方对所有带宽都提供 metered 和 unmetered 两种计费口径供选择，下单时留意自己选的是哪一种。

续费是另一个容易被含糊过去的地方。官方活动页的原话是“order now, and renew at the same price”，第三方测评也提到 LightLayer 的促销价在续费时没有上涨，用户对这点评价不错。2024 年页面上的承诺能不能延续到今天，续费账单出来才知道，但至少官方是把这句话写在明面上的。

还有一个容易踩的坑：官方条款页写明，非公司原因不支持退款，常规价产品和促销价产品都包括在内。买之前把机房、线路、带宽口径确认清楚，不要抱着“先买再退”的打算。

👉 [到结账页确认配置与价格](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74)

## 哪些人不用买 Premium

用户全在欧美，或者只是建站练手、跑 CI、做开发环境，Global 线的 $4/月完全够用，多花的两倍价钱换不来你能感知到的差别。

需要有人帮你管服务器、要 SLA 承诺、要工单秒回的，这家不合适。第三方测评对它的一致评价是：控制面板 functional but not polished，文档对复杂配置讲得不深，工单响应速度不稳定，同一机房不同节点性能有波动。$4/月的价格对应的是自助式服务，别指望托管级别的支持。

真正需要 Premium 的场景很具体：访客主要在中国大陆，或者你的应用对亚太方向的延迟和稳定性敏感。除此之外，Standard 是个中间选项，走大陆 BGP 但不含 CN2，价格比 Premium 低一档。

## 优惠码

第三方测评里出现过一些促销码，比如 2025TKYCH30OFF（日本云服务器 7 折）、2025MNLDS30OFF（菲律宾独立服务器 7 折）、HKC2M（香港云主机）、LAC2M（洛杉矶云主机）、LONC2M（伦敦云主机），还有 2026 年资料里提到的 SJCA5OFF（圣何塞）。这些码全部来自第三方，官方新闻页没有列出任何一个。

能不能用，结账页填进去当场就知道，用不了就删掉。不要因为一个码去改自己的购买决策。

## 常见问题

**$4/月的套餐带 CN2 吗？**

不带。Startup 的 $4/月是 Global 线，官方定义里 Global 只有 International BGP。要 CN2 必须选 Premium。

**Premium 一定走 CN2 GIA 吗？**

官方只写 CN2，没有区分 GIA 和 GT。第三方测评写的是 CN2 GIA + CMIN2。用上面的测试 IP 跑一遍 traceroute，比看任何文案都直接。

**年付能按原价续费吗？**

官方 2024 年活动页写的是 renew at the same price，第三方也提到促销价续费没涨。这是 2024 年页面上的表述，续费时以实际账单为准。

**优惠码在哪里填？**

结账页。第三方列出的码都没有官方确认，试填看是否生效，不生效就原价买。

**买错了能退吗？**

官方条款写明，非公司原因不退款，促销产品同样适用。

**独立服务器有 CN2 线路吗？**

促销期出现过 CN2 优化的独立服务器，价格波动很大。2025 年 6 月圣何塞双路 E5-2660 / 32GB 曾从 $648 降到 $70/月，2025 年末圣何塞 E5-2680 v4 / 32GB 约 $99/月。这类促销的配置和价格每次都不一样，以当期活动页为准。

## 最后怎么选

只要便宜、不在意大陆方向延迟，选 Startup 的 Global 档，$4/月，100Mbps 不限量。

要大陆方向低延迟，洛杉矶 Premium 是主力选项。预算宽松选年付 $49.99，预算紧就选 $24.99 的 1C/1G Premium 档，接受 20M 或 30M 的带宽上限。

用户在台湾或东南亚，台湾、马尼拉的 Premium 年付 $24.99，比洛杉矶更近。

要物理机，盯促销期的圣何塞，价格和配置每次活动都不同，别拿旧价格当参考。

下单前做两件事：ping 一遍官方测试 IP，把 Premium 和 Global 并排对比；在结账页确认带宽口径是 20M、30M 还是 100Mbps、1Gbps。这两步做完，基本不会买错。

👉 [从洛杉矶 Premium 开始核对价格](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74)
