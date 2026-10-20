# Token Plan 个人版：四档套餐价格对比与 Credits 计费规则，怎么选不花冤枉钱

Token Plan 个人版是阿里云百炼面向个人开发者推出的大模型订阅服务：按月付费，文本、多模态模型和内置工具的调用消耗统一折算成 Credits，从套餐额度里扣，额度内不用再单独付费。目前它只在中国（北京）地域开放，四档套餐限时月价从 39 元到 499 元。

先说一件容易踩坑的事：百度千帆也有一个同名的「Token Plan 个人版」，两家产品重名，但模型阵容、计费单位和折扣玩法完全不同。这篇文章以阿里云百炼的版本为主线，后面附一张对比表，帮你分清自己要买的是哪一个。

> **选购速览**
> - 轻度使用、先试水：Lite 档，限时 39 元/月，每月 11,500 Credits，日常问答和轻量编程够用
> - 每天用 AI 编程：Standard 档，限时 139 元/月，45,000 Credits，附带 AgentStudio 工具的 Harness 权益
> - 多 Agent 重度并行：Pro 档，限时 499 元/月，180,000 Credits，四档里单价最低
>
> 👉 [查看 Token Plan 个人版四档套餐的当前价格](https://bailian.console.aliyun.com/cn-beijing/subscription/token-plan/personal?userCode=5eqf8rny)

## Token Plan 个人版是什么，和逐次付费有什么区别

它是阿里云百炼的订阅制服务，核心是把模型调用和内置工具的消耗统一折算成 Credits 计费。和按 token 逐次结算相比，订阅制的成本上限就是月费，用多少都在额度内消化，预算好控制。

一份订阅覆盖的能力相当全：文本生成、推理、视觉理解、图像生成、语音合成、实时语音对话、语音识别、视频生成都在额度范围内。平台还提供一个 auto 智能路由模型，每次请求自动匹配底层模型，在质量和成本之间做平衡，不想纠结选哪个模型时直接用它。Standard 和 Pro 档另外附带 Harness 权益——AgentStudio 工具的每月免费额度和后付费折扣，这部分独立计量，不从 Credits 或加油包里扣。

## 四档套餐价格与额度对比

当前四档套餐的限时价格、额度和并发上限如下：

| 套餐 | 每月额度 | 并发 Agent | 限时月价（原价） | 订阅入口 |
| --- | --- | --- | --- | --- |
| Lite | 11,500 Credits | 1–2 个 | 39 元（原价 60 元） | [ 订阅 Lite](https://bailian.console.aliyun.com/cn-beijing/subscription/token-plan/personal?userCode=5eqf8rny) |
| Essential | 25,500 Credits | 2–3 个 | 79 元（原价 120 元） | [ 订阅 Essential](https://bailian.console.aliyun.com/cn-beijing/subscription/token-plan/personal?userCode=5eqf8rny) |
| Standard | 45,000 Credits | 3–4 个 | 139 元（原价 180 元） | [ 订阅 Standard](https://bailian.console.aliyun.com/cn-beijing/subscription/token-plan/personal?userCode=5eqf8rny) |
| Pro | 180,000 Credits | 6–8 个 | 499 元（原价 600 元） | [ 订阅 Pro](https://bailian.console.aliyun.com/cn-beijing/subscription/token-plan/personal?userCode=5eqf8rny) |

权益是逐级叠加的：Lite 包含多模态模型和内置工具；Essential 继承 Lite 全部权益；Standard 在此之上增加 Harness 权益；Pro 再加更高的并发上限。

订阅周期从下单日起算 30 天，与自然月无关。周期内累计消耗到达套餐额度，服务暂停，等下个订阅月才恢复。自己月底月初下单的人要留意——你的重置日是你付款那天，不是每月 1 号。

## Credits 怎么扣？计费规则和夜间折扣

每次请求消耗多少 Credits，由模型类型、token 用量、是否开启思考模式、是否调用工具共同决定，没有一张固定的单价表。实际消耗可以在订阅页的用量明细里逐条查看：👉 [在订阅页查看各模型的实际消耗明细](https://bailian.console.aliyun.com/cn-beijing/subscription/token-plan/personal?userCode=5eqf8rny)

扣费顺序是固定的：先扣当期订阅月的套餐额度，额度用完自动扣加油包，加油包也没有或用完就暂停服务。想继续用，要么升档，要么等下个订阅月重置。

模型折扣是目前最实在的省钱口子。每天 22:00 到次日 08:00（UTC+8）之间调用，qwen3.8-max 和 qwen3.8-flash 享受 60% off 的限时夜间折扣，deepseek-v4-pro-0813、deepseek-v4-flash-0731、deepseek-v4.1-flash 是 50% off，相当于半价。习惯晚上写代码的人，同样额度的实际产出会多出一截。另外 decision-model-preview 目前限时免费，调用不消耗 Credits。

### 额度用完了怎么办？先算清加油包的账

加油包每个 100 元/月，提供 20,000 Credits，需要在订阅有效期内购买，最多同时持有 5 个，套餐月额度用完后自动扣除。

单价值得算一笔账：加油包折合 0.005 元/Credit，而 Lite 档额度约合 0.0034 元/Credit，Standard 约 0.0031 元，Pro 约 0.0028 元。也就是说，加油包比 Lite 档贵约五成，接近 Pro 档额度单价的两倍。偶尔爆量买一两次没什么，如果每个月都靠加油包续命，升一档反而更便宜。

还有一条容易忽略的规则：**当月没用完的额度不结转**，下个周期直接按满额重置。

## 阿里云和百度千帆都叫「Token Plan 个人版」，别买混了

同名不代表同类。两家的模型、计费单位和活动逻辑都不一样，下单前先确认自己进的是哪家：

| 对比项 | 阿里云百炼 Token Plan 个人版 | 百度千帆 Token Plan 个人版 |
| --- | --- | --- |
| 入门档 | Lite：39 元/月，11,500 Credits | Mini：4.9 元/月，1,400 积分 |
| 中间档 | Essential 79 元 / Standard 139 元 | Lite 19.9 元 / Pro 99.9 元 |
| 最高档 | Pro：499 元/月，180,000 Credits | Max：299.9 元/月，165,000 积分 |
| 计费模式 | 统一 Credits 计费 | 积分制与 Token 制双轨可选 |
| 主打模型 | Qwen3.8 系列、DeepSeek-V4 系列、auto 路由 | GLM-5.2、DeepSeek-V4-Pro-0813、Kimi 等 |
| 折扣玩法 | 限时月价 + 夜间 22:00–08:00 消耗折扣 | 全时段梯度折扣：工作日白天 2 折、夜间低至 0.5 折、周末全天 1 折 |
| 工具兼容 | Claude Code、Cursor、Qwen Code、Qoder、OpenClaw | Cursor、Windsurf、Cline 等，兼容 OpenAI/Anthropic 协议 |

一个必须说清的前提：阿里云的 Credits 和百度的积分是两套单位，各平台模型的消耗速率也不同，表里的数字不能直接横比。两家甚至都有叫 Lite 的档位，额度却完全不同（11,500 Credits 对 6,600 积分）。

客观地说，只想花几块钱体验大模型订阅，百度 Mini 档 4.9 元的门槛确实更低，那边还有首购五折、首次续费六折的活动；但如果你主力工具是 Claude Code，或者明确要用 Qwen 系模型，阿里云这边的兼容列表和模型阵容更对口。

## 订阅之后怎么在编程工具里用起来

流程不长：订阅完成后，在百炼控制台创建 API Key，拿到接口地址（base URL）和密钥，然后在支持 OpenAI 或 Anthropic 协议的工具里填入这两项就能跑通。官方兼容列表明确列出了 Claude Code、Cursor、Qwen Code、Qoder、Qoder CN 和 OpenClaw。

多开 Agent 的话，并发上限跟着套餐走：Lite 1–2 个，Standard 3–4 个，Pro 6–8 个。只看额度不看并发，跑多 Agent 工作流时容易撞墙，两个数要一起核。

## 什么人适合订，什么人先别急

按用量对号入座：

- **Lite（39 元/月）**：每月用量在一万 Credits 上下的轻度用户。夜间折扣还能再放大实际产出。👉 [从 Lite 档开始试水](https://bailian.console.aliyun.com/cn-beijing/subscription/token-plan/personal?userCode=5eqf8rny)
- **Standard（139 元/月）**：每天靠 AI 编程干活、会用 AgentStudio 工具的人。Essential 和 Standard 的额度单价几乎一样（都约 0.0031 元/Credit），差在总量和 Harness 权益——月用量稳定在 25,500 到 45,000 之间、又不需要 AgentStudio 工具，选 Essential 能省 60 元；否则 Standard 更值。
- **Pro（499 元/月）**：多 Agent 常年并行、用量经常打满 45,000 的重度用户。180,000 Credits 是 Standard 的四倍，价格只有它的 3.6 倍，单价最低。

视频生成重度用户要克制：单次消耗随时长和分辨率上涨，可能一口气吃掉大块额度，而且异步任务是完成后批量结算，短时间提交多个任务，完成后的集中扣费可能直接把额度打到暂停线。

两种情况建议先缓一缓。一是你不在北京地域——中国版只在北京地域提供，海外用户对应的是新加坡地域的国际版，按美元计价，Lite 限时 6 美元/月起。二是你的月用量远低于 11,500 Credits，那先从最低档试一个月，看到真实消耗再决定升不升档，比拍脑袋估靠谱。

## 常见问题

**额度每月怎么重置？没用完的能攒吗？**
每个订阅月（从订阅日起 30 天）开始时自动恢复到所属套餐的满额，没用完的不结转。2026 年 9 月 22 日平台取消周额度时，存量订阅在当天按套餐完整月额度统一重置了一次，订阅周期和到期时间都没变。

**能一天提交多个视频生成任务吗？**
能，但要清楚结算机制：异步任务的 Credits 在任务完成后才扣，不是提交时扣。短时间堆多个任务，完成后的集中结算可能一次性消耗大量额度。

**加油包能囤几个？**
最多同时持有 5 个，且必须在订阅有效期内购买。套餐月额度用完后，加油包 Credits 自动扣除。

**支持哪些编程和 Agent 工具？**
官方列出 Claude Code、Cursor、Qwen Code、Qoder、Qoder CN、OpenClaw。走 OpenAI 或 Anthropic 协议的主流工具一般也能接入，配置 base URL 和 API Key 即可。

## 下单前最后确认两件事

一，重置日。订阅周期从付款那刻起算 30 天，额度不结转，把开通时机放在自己用量高峰前最划算。二，地域。中国版只在北京地域，账号和工具环境先对上，海外需求看国际版。

选档的判断标准就一条：按真实月用量匹配额度，轻度用选 Lite，日常编程选 Standard，重度并行选 Pro，在 Essential 和 Standard 之间纠结时记住两者单价几乎一样、差在 Harness 权益。👉 [订阅 Token Plan 个人版](https://bit.ly/aliyun-coupon)
