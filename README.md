# Problem Framing 提示词

用 AI 生成规范的 Problem Framing，适用于 Claude、ChatGPT、Gemini 等任意 AI 工具。

---

## 什么是 Problem Framing？

Problem Framing 是一种产品思维方法，帮助你在定义需求之前，先把"用户问题"说清楚。

核心句式：

> **[WHO]** 在 **[WHEN]** 时，面临 **[WHAT problem]**。他们希望 **[WHAT job]**。
> 我们的方案需要帮助 **[Customer Benefits]**，同时实现 **[Business Benefits]**。

写好 Problem Framing 的关键有两点：
- **去方案化**：Benefits 只描述"理想结果"，不出现具体的功能、UI 或技术手段
- **用户口吻**：problem 和 job 站在用户视角描述，让读者产生共情

---

## 使用方法

### 方式一：直接复制提示词（适用于任意 AI 工具）

把下方提示词复制到你使用的 AI 工具里，然后粘贴你的项目描述即可。

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

### 方式二：安装为 Claude Skill（适用于 Claude.ai）

下载 [`problem-framing.skill`](./problem-framing.skill) 文件，在 Claude.ai 中上传安装。安装后，直接对 Claude 说"帮我写 Problem Framing"即可触发。

---

## 输出示例

**输入：** 用户在首页浏览完商品详情回来后，首页内容和他刚看的东西没什么关系，想解决这个问题。

**输出：**

浏览完商品详情回到首页的用户（WHO），在退出商品页回到首页的瞬间（WHEN），发现首页内容和他们刚才看的东西相关性不大，导致他们的探索和购物意愿减弱（WHAT problem）。他们希望首页可以及时响应当前的兴趣、展示一些相关内容，让他们可以更方便地继续探索类似商品（WHAT job）。
我们的方案需要提升用户此时在首页的浏览和购物体验的相关性与及时性（WHAT benefits for the customer），并最终提升首页的 GMV sku per UV（WHAT benefits for the company）。

---

更多示例见 [`examples.md`](./examples.md)。

---

## 文件说明

| 文件 | 说明 |
|------|------|
| `README.md` | 使用说明（本文件） |
| `prompt.md` | 完整提示词，方便复制 |
| `examples.md` | 4 个完整示例 |
| `problem-framing.skill` | Claude.ai Skill 安装包 |

---

## 贡献

欢迎提 Issue 或 PR，分享你在其他场景下写的 Problem Framing 示例。
