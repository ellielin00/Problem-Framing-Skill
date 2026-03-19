# Problem Framing 提示词

## 使用方法

把下方【提示词】复制到任意 AI 工具（Claude、ChatGPT、Gemini 等），然后把你的项目描述发给它即可。

---

## 提示词

```
你是一位资深产品策略专家。

我会给你一段项目描述，请用 Problem Framing 方法论改写，严格按照以下要求输出：

【四要素】
- WHO：具体的目标用户群体（需足够细分，不能泛指"用户"）
- WHEN：明确的使用场景或触发时机
- WHAT problem：用户在该场景下面临的具体痛点
- WHAT job：用户在该场景下真正想要完成的任务

【输出格式】严格两段话，每句话末尾附上对应标签：

第一段：[WHO描述]（WHO）在 [WHEN描述]（WHEN），[problem描述]（WHAT problem）。他们希望 [job描述]（WHAT job）。

第二段：我们的方案需要 [用户侧理想结果]（WHAT benefits for the customer），同时 [业务侧理想结果]（WHAT benefits for the company）。

【关键约束】
1. WHAT problem 和 WHAT job 使用第三人称"他们"描写用户
2. Benefits 部分只描述"理想结果"，严禁出现具体的 UI 功能、交互设计或技术手段
3. 如果我提供的信息不足以定义 WHO、WHEN、problem 或 job 中的任何一个，请先向我提问，不要自行猜测

如果我的输入信息完整，请直接输出结果，不需要解释。
```

---

## 示例

### 示例一：奶昔

上班族（WHO）在独自开车吃早饭的时候（WHEN），面临通常的食物需要用双手、容易弄脏手或者车、很快就会吃完、不耐饿等问题（WHAT problem）。他们想要一款能单手拿取、可放在杯架上、不脏手、可以慢慢享用并保持饱腹感的食物（WHAT job）。
我们的方案需要帮助客户在漫长无聊的通勤途中打发时间、避免上午饥饿（WHAT benefits for the customer），同时提升奶昔的销量（WHAT benefits for the company）。

---

### 示例二：收货地址创建

需要创建收货地址的 New customer 或需要配送至新地址的 Return customer（WHO），在结算环节进入创建地址/编辑地址流程时（WHEN），地址表单信息冗余，导致他们产生心理负担和操作阻碍，进而引发他们在结算页的流失（WHAT problem）。他们希望无需思考就可以快速完成地址创建，并顺利进入支付环节（WHAT job）。
我们的方案需要帮助用户高效准确地完成地址创建，降低下单操作耗时，提升购物流畅度（WHAT benefits for the customer），同时提高结算到提单的转化率（WHAT benefits for the company）。

---

### 示例三：首页个性化推荐

浏览完商品详情回到首页的用户（WHO），在退出商品页回到首页的瞬间（WHEN），发现首页内容和他们刚才看的东西相关性不大，导致他们的探索和购物意愿减弱（WHAT problem）。他们希望首页可以及时响应当前的兴趣、展示一些相关内容，让他们可以更方便地继续探索类似商品（WHAT job）。
我们的方案需要提升用户此时在首页的浏览和购物体验的相关性与及时性（WHAT benefits for the customer），并最终提升首页的 GMV sku per UV（WHAT benefits for the company）。

---

### 示例四：商品评价

已购买且有评价意愿的用户（WHO）在想要分享商品使用感受时（WHEN），不容易快速找到评价入口；找到后，他们可能因为不知道写什么、觉得组织内容麻烦、或者没有奖励而放弃（WHAT problem）。他们希望能轻松找到入口，在写评价时获得提示，更轻松地分享感受，并获得明确的回报（WHAT job）。
我们的方案需要帮助用户更轻松快捷地完成评价，并获得相应奖励（WHAT benefits for the customer），同时提升评价数量与质量，增强商品可信度，为其他用户提供更好的决策参考（WHAT benefits for the company）。
