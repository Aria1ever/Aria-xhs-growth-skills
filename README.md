# 小红书获客 · 矩阵占位 Skill 体系（客资版）

![小红书获客 Skill 体系一览](assets/skill-overview.png)

---

## 这个Skill 解决什么

多账号获客卡住的地方通常是三个：号和号之间词组重叠互相抬价、内容没有分工发着发着就重了、AI 写出来没有真情实感。

这套 Skill 体系按流程分工，三个 Skill 各成一个小组：

| Skill | 管哪一段 | 解决什么 |
|---|---|---|
| `matrix-placement` | 起号规划 | 多账号按词分工，不撞车、不同质 |
| `cover-title` | 每篇封面+标题 | 现查活数据源，找当下有效结构，不套过期公式 |
| `xhs-content-writing` | 正文写作 | 写出"真实的人在说话"的内容，建立信任 |

---

## 安装

在 Claude Code 终端里按需安装：

```bash
# 矩阵占位规划师
claude skills add github:Aria1ever/Aria-xhs-growth-skills/skills/matrix-placement

# 封面标题生成器
claude skills add github:Aria1ever/Aria-xhs-growth-skills/skills/cover-title

# 获客文案写作引擎
claude skills add github:Aria1ever/Aria-xhs-growth-skills/skills/xhs-content-writing
```

---

## 怎么用

**标准流程（三步接力）：**

```
matrix-placement
输入：产品信息 + 账号数量 + 投流现状 + 成交痛点
输出：账号分工占位表 + 占位覆盖地图 + 跨平台改写指引
       ↓
cover-title
输入：行业 + 矩阵分线（L1-L6）+ 标杆封面
输出：3-5 组封面文案 + 标题，标注迁移来源和视觉建议
       ↓
xhs-content-writing
输入：分线 + 账号人设 + 产品信息
输出：定位 → 情绪弧线正文 → 说人话校对
       ↓
发布 · 投流 · 接询盘
```

**单独用也行：**
- 只想规划矩阵 → 只装 `matrix-placement`
- 只想改封面标题 → 只装 `cover-title`
- 只想去 AI 腔 → 只装 `xhs-content-writing`，直接跳「说人话引擎」那一段

---

## Skill 地图

从起号到复盘的整条客资链路。分三层：

**核心层 · 客资骨架**

| Skill | 干什么 | 状态 | 来源 |
|---|---|---|---|
| matrix-placement | 矩阵占位表（含跨平台改写、素材去重） | ✅ 开源可跑 | 本人 |
| cover-title | 封面标题（对接矩阵分线，高点击不靠焦虑，现查活数据源） | ✅ 开源可跑 | 本人 |
| 聚光投流复盘 | 投流数据直接给结论，写进禁用词库 | 行业定制 | 本人 |
| feishu-cli | Obsidian 写好，一行命令变飞书云文档 | 展示 | riba2534 |
| 马斯克时间管理 | 五连问砍掉不该存在的事，多号提效 | 展示 | alchaincyf |
| 归因分析（原 ab-test） | 两版选哪个，给决策依据不给感觉 | 展示 | phuryn/pm-skills |

**生产力层 · 话术与认知**

| Skill | 干什么 | 状态 | 来源 |
|---|---|---|---|
| AI HOT | 30 秒一份 AI 圈简报，客资博主的选题弹药 | 展示 | aihot.virxact.com |
| 写作分身（Aria2ever） | 见字如面的写作 Skill | 🔓 说人话试用版开源 · 完整版不开源 | 本人 |
| huashu-design | 把脑子里的想法变成可展示的图/PPT | 可选 | alchaincyf |

**沉淀层 · 让流程自己长**

| Skill | 干什么 | 状态 | 来源 |
|---|---|---|---|
| skill-creator | 把"搓 Skill"这件事本身做成 Skill | 内置 | Anthropic |
| darwin-skill | 9 维打分，让 Skill 像模型一样自己迭代 | 展示 | alchaincyf |

---

## 关于写作 Skill 的开源范围

`xhs-content-writing` 包含完整的方法论框架（他者的面孔信任体系 + 说人话引擎），开源可跑。

完整版 `Aria2ever` 学过赵赵所有的文字、读过的书、判断方式，是见字如面的写作分身。

---

📎 交流更多：
<img width="888" height="1131" alt="71c0a952c8f903e71df3d6cafdfff78f" src="https://github.com/user-attachments/assets/b6d4e2d1-d4eb-4004-8df6-c835370d700b" />


_作者：赵赵 Aria
