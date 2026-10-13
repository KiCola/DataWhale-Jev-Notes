---
research-card: true
title: "DataWhale-Jev Cookbook 研学"
status: "进行中"
color: "#8aab6b"
updated: "2026-10-08"
---
# DataWhale-Jev Cookbook 研学
开源教程：jev cookbook（从零入门 Jev）
**课程简介
本次共学围绕 JEV Cookbook** 展开，第一期以 **JEV 基础认知、核心原语、Cookbook 实战与基础评测** 为主。课程不追求一次性覆盖全部进阶内容，而是帮助大家先建立对 JEV 的基本理解，掌握 Choice / Score / Noul 三种核心问题原语，并通过真实案例理解 JEV 在分类、排序、路由、判断等任务中的使用方式。**
学习形式以：教程阅读 + Notebook 实验 + 简单改造 + 学习总结 为主。第一期暂不重点展开 Agent 深度集成、Laya、本地模型、RLCD 微调等进阶内容，降低第一次学习门槛，优先保证大家能够跑通、理解并实际使用 JEV。
**适合人群：适合有一定 Python 基础，对 JEV、System One Model 感兴趣，希望通过实战探索分类、路由、Tool Selection 等任务在 LLM / Agent / RAG 应用中如何实现的同学。**
https://github.com/datawhalechina/jev-cookbook
https://docs.typesafe.ai/primitives/noul
## 项目研究
https://datawhalechina.github.io/jev-cookbook/
大语言模型（LLM）的设计目的是生成供人类阅读的文本。当你需要模型做出一个供代码消费的判断时，就产生了错位：你在强迫一个文本生成系统输出结构化决策，然后再把结果解析回代码可以依赖的形式。
Jev 是 TypeSafe 的旗舰模型，也是首个 [System One 模型](https://datawhalechina.github.io/jev-cookbook/concepts/system-one/)。System One 模型专为做出软件可直接使用的快速结构化决策而构建。Jev 针对状态评估类型化问题，并直接返回结构化结果。没有文本生成，也无需解析。你得到的是类型化的值和概率分布，代码可以据此进行分支、排序和路由。Choice 和 Score 还会返回[置信度](https://datawhalechina.github.io/jev-cookbook/confidence/)，你的代码可以用它来决定是否行动以及如何行动。
![[file-20261008162126147.png]]
### TypeSafe Jev 试用
[https://datawhalechina.github.io/jev-cookbook/introduction/quickstart/#%E8%AF%95%E7%94%A8playground](https://console.typesafe.ai/playground)
![[file-20261008162400536.png]]
![[file-20261008162444201.png]]
TypeSafe 是真的在教你怎么试用Jev
![[file-20261008162607847.png]]![[file-20261008162755510.png]]
### 范式更新
![[file-20261008163714838.png]]
![[file-20261008163851369.png]]![[file-20261008165628929.png]]
代码负责确定性工作并掌控控制流。模型只出现在系统需要可编程的常识、或需要解读非结构化数据的地方。每个 AI 任务都保持原子性并受到约束。
![[file-20261008165827472.png]]

## 多模态Jev
https://mp.weixin.qq.com/s/tabPKzFy73bTmTBs9OyUVw?poc_token=HAdfx2qjrN5tveWUlo_JgPgEupzGiesV95lg7BrJ

## 多模态VLM-Jev
