# 小红书获客 · 矩阵占位 Skill 体系（客资版）

> 不是教你怎么涨粉的博主版。是教你怎么用一批号，把目标词占满、把获客成本压下来的客资版。

![小红书获客 Skill 体系一览](assets/skill-overview.png)

---

## 总 · 用小红书做获客，死在哪里

博主账号和客资账号，目标函数根本不同：

**博主账号**：涨粉 → 被品牌看见 → 接广告  
**客资账号**：占词 → 被客户搜到 → 引询盘 → 成交

做获客的号，衡量标准不是粉丝数，是每一个来询的**客资成本**。

多账号获客卡住的位置通常有三个：

| 卡点 | 症状 |
|---|---|
| 账号层 | 多个号全在抢同一个大词，互相把投流成本抬高 |
| 内容层 | 没有分工逻辑，号和号发着发着内容就重了 |
| 语言层 | AI 生成的帖子一眼看出来，高净值客户防御心直接拉满 |

这套 Skill 体系专门解这三件事，分两个模块：

| 模块 | Skill | 解决什么 |
|---|---|---|
| 账号层 | `matrix-placement` | 多账号分工：每个号占不同的词组和内容线，不撞车 |
| 内容层 | `xhs-content-writing` | 写出「真实的人在说话」的获客帖，建立信任 |

两个 Skill 在流程上接得住：先用矩阵规划确定每个号"占什么词 / 走什么线"，再用写作引擎产出符合那条线的内容。

---

## 分 · 两个 Skill 详解

### Skill 01 · matrix-placement · 矩阵占位规划师

```bash
claude skills add github:Aria1ever/Aria-xhs-growth-skills/skills/matrix-placement
```

**解决的问题**：同一个大词，多个号在竞争。投流成本高、自然流不集中、内容同质化。

**输入六项，缺一项它会停下来问你**：

| 字段 | 说明 |
|---|---|
| 产品 / 品牌 | 是什么、白牌还是有品牌资产 |
| 客单价 / 人群 | 高净值还是泛人群，决策成本高低 |
| 账号数量 | 几个号（默认 5 个） |
| 投流现状 | 哪些号在投、投什么词 |
| 目标平台 | 只做小红书还是多平台 |
| 成交痛点 | 客户最常卡在哪一步 |

**固定输出三张表**：

- **表一 · 账号分工占位表**：每个号各占哪些词、走哪条内容线、5 个不重样的角度
- **表二 · 占位覆盖地图**：验证没漏词、号间没撞车
- **表三 · 跨平台改写指引**（多平台时出）

同样的需求，裸跑 Claude 给你按"风格"分账号，挂上这个 Skill 给你按"词面"分账号。词面一旦分死，号之间天生不同质化。

→ 完整文档：[skills/matrix-placement/SKILL.md](skills/matrix-placement/SKILL.md)

---

### Skill 02 · xhs-content-writing · 获客文案写作引擎

```bash
claude skills add github:Aria1ever/Aria-xhs-growth-skills/skills/xhs-content-writing
```

**解决的问题**：内容写出来一看就是 AI 写的，或者措辞像在卖货，高净值客户划走。

**三段式流程**：

```
① 定位  →  他者的阶级光谱 + 四步定位法
           找准读者、定好"写作面孔"和决策开关

② 下笔  →  情绪弧线
           相似感开场 → 当事人那句话 → 开口子
           （有真实拦截点时，中间加 Q&A）

③ 校对  →  说人话引擎
           去 AI 腔黑话 / 去销售腔 / 去官腔 / 说完就走
```

核心命题来自列维纳斯：**信任不来自权威，来自他者的面孔。** 当读者看见一张和自己处境相似的面孔，防御自动降下来。

**适用赛道**：子女国际教育 / 留学 / 移民 / 医美 / 财富管理 / 高端消费品

**两种使用方式**：
- 写一篇获客帖：三段式走全程（定位→下笔→校对）
- 只想去 AI 味：直接跳到第三段「说人话引擎」，把现成文字丢进去改写

→ 完整文档：[skills/xhs-content-writing/SKILL.md](skills/xhs-content-writing/SKILL.md)

---

## 总 · 完整获客工作流

```
有产品 / 有获客需求
       ↓
matrix-placement
给多账号分工：A 号占避坑词 / B 号占信任词 / C 号占对比词...
       ↓
xhs-content-writing
给每条线写内容：定位（面孔+开关）→ 下笔（情绪弧线）→ 校对（说人话）
       ↓
发布 · 投流 · 接询盘
```

---

## 四条使用前提

1. **占词占位 > 发爆款。** 白牌在小红书的地基是把搜索词占满，不是靠某篇爆文。爆款锦上添花，占位才是活下来。

2. **跨平台不是搬运，是各自重做。** 小红书、抖音逻辑根本不同，同一卖点要按平台重写，绝不"一稿多发"。

3. **素材重复是管理问题，不是产能问题。** 缺的不是更多素材，是分工。分线定死，号间天然不撞车。

4. **AI 接 1→10，0→1 得你自己想清楚。** 人群画像、成交痛点这些前提错了，矩阵铺得越快错得越齐。

---

## 谁适合 / 不适合

**适合**：手里有多个号，靠搜索和投流获客，卡在"铺不出分工 / 素材重复 / 获客太贵"的人。电商白牌、高净值定制类（装修 / 留学 / 医美等）都跑得通。

**不适合**：想做一个有人设的博主号去接广告的人，那是另一条路，这套帮不上。

---

## 十个 Skill 安装指南

对应小红书文章里的 10 个 Skill，分三层。在 Claude Code 终端里按需安装：

**核心层 · 客资骨架**（直接影响获客效率）

```bash
# 矩阵占位规划师 · 本仓库
claude skills add github:Aria1ever/Aria-xhs-growth-skills/skills/matrix-placement

# 获客文案写作引擎 · 本仓库
claude skills add github:Aria1ever/Aria-xhs-growth-skills/skills/xhs-content-writing

# 飞书推送 · riba2534 出品
claude skills add github:riba2534/feishu-cli

# 时间管理（马斯克模式）· alchaincyf 出品
claude skills add github:alchaincyf/elon-musk-skill

# 归因分析（A/B 决策）· phuryn 出品
claude skills add github:phuryn/pm-skills
```

聚光投流复盘：内部工具，本仓库暂不开放。

**生产力层 · 选题与设计**

```bash
# AI 选题简报（AI HOT）· 访问官网按说明安装
# https://aihot.virxact.com

# 设计出图（huashu-design）· alchaincyf 出品
claude skills add github:alchaincyf/huashu-design
```

xhs-content-writing 即 Aria2ever 的开源方法论版，可直接安装。

**沉淀层 · 让流程自己长**

```bash
# Skill 自迭代（darwin-skill）· alchaincyf 出品
claude skills add github:alchaincyf/darwin-skill

# skill-creator：Claude Code 内置，直接输入 /skill-creator 使用，无需安装
```

---

## 关于写作 Skill 的开源范围

`xhs-content-writing` 包含完整的方法论框架（他者的面孔信任体系 + 说人话引擎），开源可跑。

完整版 `Aria2ever` 学过赵赵所有的文字、读过的书、判断方式，是见字如面的写作分身。

---

📎 交流更多：
<img width="888" height="1131" alt="71c0a952c8f903e71df3d6cafdfff78f" src="https://github.com/user-attachments/assets/b6d4e2d1-d4eb-4004-8df6-c835370d700b" />


_作者：赵赵 Aria
