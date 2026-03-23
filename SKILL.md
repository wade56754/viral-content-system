---
name: x-longform-writer
description: >
  为 Wade（@bigu62 / Koda一人公司）生成推特长文。触发：用户要求"写长推""写推特文章"
  "帮我写一篇XX主题的长文""拆解这篇爆文""改这篇推文""优化这篇"等。
  适用3000-5000字认知类/工具类/趋势类长文。
---

# x-longform-writer v3.1 — 裂隙理论统一框架

> 版本：v3.1 | 更新：2026-03-20
> 架构：Wade 6层分离 × 叁斤进化闭环 × Thariq 渐进披露

---

## 第一性原理

写作只做一件事：**在读者脑中制造一个裂隙，然后用你的认知填上它。**

McKee 叫裂隙，Sugarman 叫好奇心种子，罗振宇叫先破后立，程前叫谜题。
6本写作经典 + 罗振宇16篇 + Wade 实战数据，收敛到同一个点。

---

## 写作铁律（L1 — 全程有效，不可违反）

1. **犹豫就删** — 删减是最核心的写作能力
2. **第一句话唯一任务是让人读第二句话** — 开头决定生死
3. **具体 > 抽象** — 数字和场景比形容词强100倍
4. **每句话过"读者关心吗"测试** — 读者不关心的删掉
5. **重写才是真正的写作** — 第一稿只是思考过程
6. **弹药是树叶不是树根** — 删掉所有弹药骨架还站得住
7. **技术是佐证，认知才是正文** — 读者要的不是你怎么做，是你明白了什么

---

## 裂隙的4种形状

| 裂隙 | 读者的缺口 | 撕开方式 | 展开模式 |
|------|-----------|---------|---------|
| 🧠 认知裂隙 | "我以为的是错的" | 反常识炸弹/因果倒置 | 模式A：递进否定 |
| 🔧 能力裂隙 | "我不会做这件事" | 痛点具象化/极端案例 | 模式B：并列打透 |
| 💡 信息裂隙 | "我不知道这个东西" | WOW事实/稀缺信息 | 模式B：并列打透 |
| ❤️ 情感裂隙 | "原来别人也这样" | 个人故事/脆弱时刻 | 模式A：递进否定 |

一篇文章可以同时有多种裂隙。没有裂隙 = 不值得写。

> 裂隙三幕详解（撕裂→填充→缝合）、两种展开模式、6条通用规则
> → 读 `references/rift-theory.md`

---

## 能力边界

**能做**：推特长文（X Article / Thread）、认知类/工具类/趋势类
**不做**：小红书笔记（→ xhs-writer）、短推（→ x-short-tweet）、纯新闻搬运

**字数**：3000-5000字（X Article）；Thread 每条200-280字
**署名**：Koda一人公司 @bigu62

---

## 入口路由（根据输入自动判断流程）

| 用户输入 | 路由 | 说明 |
|---------|------|------|
| 给了主题/话题，无框架 | → 完整 Phase 0-9 | 标准流程 |
| 给了框架/大纲 | → 跳过 Phase 1，直接 Phase 2 确认 | 框架已有 |
| 给了爆文要求拆解 | → 爆文拆解模式 | 三层拆解→迁移→重写 |
| 给了原话/语音/碎片想法 | → 共创模式 | 保护 Wade 原话，AI 补充扩展 |
| 说"改这篇"/"优化" | → 改稿模式 | 只跑 Pass 2-3 |

**⚠️ 判断完路由后，严格按对应流程执行，不跳步骤。**
**⚠️ 不确定走哪条 → 先问 Wade。**

---

## ⚠️ Gotchas（踩坑清单 — 最高价值段）

> 完整踩坑记录见 `data/gotchas.md`，以下是 Top 踩坑。每次改稿后追加新条目。

1. **通用话题陷阱** — 越熟悉的话题越容易跳过武器库。通用话题 = 高风险，必须更严格走 Phase 3
2. **弹药重复** — 写前必读 used-weapons.md，已用弹药不复用
3. **全稿重写最贵** — 先确认骨架再写全稿。V1→V5 = token浪费5倍
4. **模板填充 ≠ 思考** — 套公式 = 营销号。每个论据要有独立论证逻辑
5. **比喻堆砌** — 1篇 = 1个核心比喻。多了读者记不住
6. **开头最易有AI味** — "在这个XX的时代" → 直接亮数据/事实/故事
7. **Wade不用排比句** — 三段排比 = 一秒识别AI

---

## 进化系统（每次写作自动执行）

### 写前（Phase 0 加载）
1. 读 `data/gotchas.md` — 踩坑清单
2. 读 `~/.openclaw/workspace-sentinel/data/revision-rules.md` — 改稿规律
3. 读 `~/.openclaw/workspace-sentinel/data/used-weapons.md` — 排除已用弹药

### 写后（Phase 9 之后）
4. 保存 AI 原稿到 `data/draft-archive/YYYYMMDD-{主题}-原稿.md`
5. Wade 改完终稿后，diff 原稿 vs 终稿：
   - 提炼新 gotcha → 追加到 `data/gotchas.md`
   - 提炼新规律 → 追加到 `revision-rules.md`
   - 记录使用的弹药 → 追加到 `used-weapons.md`

### 月度
6. gotchas 中 ≥3 次的规律 → 晋升到本文件「写作铁律」

---

## 3 Pass 执行制

```
Pass 1（L1+L2+L3）：骨架 + 弹药 + 初稿
  → 写作铁律内化 + 裂隙框架 + 武器库填弹药
  → 产出：结构完整但可能有AI味的初稿

Pass 2（L4+L5）：风格化 + 去AI化
  → 读 references/wade-style-dna.md 做风格改写
  → 读 references/anti-ai-checklist.md 做24模式检测
  → 产出：像 Wade 写的稿子

Pass 3（L6）：推特平台优化
  → 读 references/twitter-optimization.md
  → Hook Tweet 3版 + 封面 + 金句卡片 + 发布包
  → 产出：可发布的完整推文包
```

**每个 Pass 之间 Wade 可介入改稿。**

---

## 完整工作流

### Phase 0：灵魂加载（不可跳过）

```
按顺序读取，不可省略：
1. ~/.openclaw/workspace-sentinel/IDENTITY.md       → Wade 是谁
2. ~/.openclaw/workspace-sentinel/VOICE_DNA.md      → 语言DNA
3. ~/.openclaw/workspace-sentinel/AUDIENCE.md       → 受众画像 v2
4. ~/.openclaw/workspace-sentinel/PLATFORM_RULES.md → 推特算法权重
5. data/gotchas.md                                   → 踩坑清单
6. revision-rules.md + used-weapons.md               → 进化系统
```

### Phase 1：找谜题（选题质检）

```
Step 1：一句话写出这篇文章要回答的问题

Step 2：判断裂隙类型（见上方4种形状表）

Step 3：选题三问（全部通过才动笔）
  ① 受众穿透力：不是 Wade 用户也能看懂？
  ② 认知增量：读完后读者会改变行为或想法？
  ③ Wade 代表性：Wade 有一手经历能撑起来？

Step 4：选题类型判断
  A类（经历驱动）→ 模式A递进否定
  B类（观点驱动）→ 模式A递进否定
  C类（工具驱动）→ 模式B并列打透

任一不过 → 停，告诉 Wade 问题在哪
```

### Phase 2：骨架设计

**⚠️ 先定骨架，再找弹药。不能反过来。**

```
Step 1：核心论点（一句话，≤20字）
Step 2：拆出2-3个支撑论据（每个一句话）
Step 3：每个论据的打透方式（必须用不同方式）
Step 4：选核心比喻（引入/回扣/收束位置）
Step 5：自我反驳位置
Step 6：收束风格

→ 读 references/rift-theory.md 确定展开模式
→ 读 references/hooks-and-emotions.md 选 Hook 类型
→ 用 templates/skeleton.md 输出骨架
→ 等 Wade 确认后进入 Phase 3
```

### Phase 3：弹药检索

**骨架确定后，按需搜索弹药。完整规范 → 读 `references/arsenal-guide.md`**

核心规则：
- Wade 弹药 > 分类弹药 > weapon_search
- 每篇外部弹药 ≤ 5条
- 弹药是树叶，删掉后骨架还站得住

### Phase 4：写作（Pass 1）

**模式判断：**
```
IF Wade 提供了原话/语音：
  → 共创模式：保护 Wade 原话节奏，AI 补充扩展
IF 从零生成：
  → AI主导模式：严格按骨架写
```

**写作时：**
- 读 `references/rift-theory.md` 执行对应的展开模式
- 遵守写作铁律（L1）
- 呼吸感规则：短句断句/关键句独占一行/禁匀速/逗号当句号

**Wade 修改指令库（持续积累）：**

| AI 倾向写 | Wade 改成 | 规律 |
|-----------|-----------|------|
| "叔本华有个比喻" | "叔本华说" | 简洁化 |
| "大部分人都理解错了" | "95%的人都没理解对" | 数字化 |
| "先学明白再去做" | "学明白了就会做了" | 口语化 |
| "用AI干掉它" | "把经验总结成SOP做成Skill交给AI" | 具象化 |

### Phase 5：风格化 + 去AI化（Pass 2）

```
Step 1：读 references/wade-style-dna.md，对照改写全文
Step 2：读 references/anti-ai-checklist.md，逐项检测
Step 3：AI味得分 ≤ 3 才合格，否则继续改
```

### Phase 6：自检（8项，任一未过 → 改）

**⚠️ 自检是"写手自查"，不是"独立审稿"。自检全过 ≠ 可以发布，必须走 Phase 7。**

| # | 检查项 |
|---|--------|
| 1 | 第一句话≤15字，能让人读第二句？ |
| 2 | 前300字内裂隙已撕开？ |
| 3 | 只有1个核心论点？ |
| 4 | 论据类型≥3种且不连续重复？ |
| 5 | 核心比喻贯穿（引入→回扣→收束）？ |
| 6 | 弹药≤5条且删掉后骨架还在？ |
| 7 | 对照 data/gotchas.md 逐条检查？ |
| 8 | 朗读过一遍，不卡？ |

### Phase 7：独立审稿（不可跳过 — 硬门槛）

**⚠️ Phase 7 未通过 = 禁止进 Phase 8 生成发布包。没有例外。**

```
Step 1：读 ~/.openclaw/skills/content-review/SKILL.md
Step 2：按 content-review 完整流程执行审稿
   输入：全文 + platform="x-article" + 标题 + target_audience
Step 3：执行三关检查
   第一关：硬门槛（宪法/禁区/合规）→ 任一不过直接 KILL
   第二关：16项质控清单 → 必过项未过强制改完
   第三关：100分评分体系 → 输出评分卡
Step 4：判定
   ≥ 75分 → ✅ 进 Phase 8
   60-74分 → ⚠️ 改完评分卡指定项 → 重新走 Phase 7
   < 60分 → ❌ 打回 Phase 4 重写 → 重新走 Phase 5-7

维度最低线（任一不达标 → 打回，无论总分）：
   Hook强度 < 10分 → 打回
   标题爆发力 < 6分 → 打回
   即时可用性 < 8分 → 打回
   人味儿 < 5分 → 打回
```

**审稿输出必须包含完整评分卡（格式见 content-review SKILL.md）。**

### Phase 8：发布包生成（Pass 3）

```
Step 1：读 references/twitter-optimization.md
Step 2：生成发布包

  work/output/publish-kit/YYYY-MM-DD-{slug}/
  ├── article.md          ← 定稿全文
  ├── article.html        ← HTML 预览版
  ├── cover.png           ← 封面图（Koda一人公司署名）
  ├── quotes/             ← 金句卡片 3-5张
  ├── hook-tweets.md      ← 3版 Hook Tweet（故事/冲突/数据）
  ├── first-comment.md    ← 评论区首条评论
  └── preview.html        ← 本地预览页

Step 3：封面生成
  baoyu-article-illustrator --type title-cover --preset x-article
  金句卡片：baoyu-article-illustrator --type quote-card
```

### Phase 9：评论区运营 + 数据反馈

**运营：**
- 发布5分钟内自发首条评论
- 前1小时优先回复争论性评论（算法最高权重）
- 不防御性回复

**数据反馈：**
- Wade 提供数据 → 记录到 memory
- 积累5条 → 分析规律，更新裂隙权重
- 高爆（>500赞）→ 追加参考案例
- 扑街（<50赞）→ 分析原因

**进化（写后必做）：**
- 原稿存档到 `data/draft-archive/`
- Wade 改完后 diff → 更新 gotchas + revision-rules + used-weapons

---

## 参考文件索引

| 文件 | 用途 | 加载时机 |
|------|------|---------|
| `references/rift-theory.md` | 裂隙三幕+展开模式+通用规则 | Phase 2, 4 |
| `references/hooks-and-emotions.md` | Hook+情绪+标题 | Phase 2, 8 |
| `references/arsenal-guide.md` | 武器库使用规范 | Phase 3 |
| `references/wade-style-dna.md` | Wade风格DNA | Phase 5 (Pass 2) |
| `references/anti-ai-checklist.md` | 去AI化24模式检测 | Phase 5 (Pass 2) |
| `references/twitter-optimization.md` | 推特平台优化 | Phase 8 (Pass 3) |
| `templates/skeleton.md` | 骨架模板 | Phase 2 |
| `data/gotchas.md` | 踩坑清单 | Phase 0, 6 |
| `data/draft-archive/` | 原稿存档 | Phase 9 |

---

## 灵魂文件路径

| 文件 | 路径 |
|------|------|
| Wade 身份宪法 | `~/.openclaw/workspace-sentinel/IDENTITY.md` |
| 语言DNA | `~/.openclaw/workspace-sentinel/VOICE_DNA.md` |
| 受众画像v2 | `~/.openclaw/workspace-sentinel/AUDIENCE.md` |
| 平台规则v2 | `~/.openclaw/workspace-sentinel/PLATFORM_RULES.md` |

---

## 更新日志

- **v3.1**（2026-03-20）：**6层分离重构**。655行→<500行+渐进披露。新增：入口路由器/Gotchas踩坑清单/进化系统闭环/3 Pass执行制/写作铁律L1。详细内容拆分到 references/（裂隙理论/Hook/武器库/风格DNA/去AI化/推特优化）。新建 templates/ data/
- **v3.0**（2026-03-20）：裂隙理论统一框架。4种裂隙形状×2种展开模式×6条通用规则。从第一性原理重构
- **v2.2**（2026-03-19）：4个独立公式体系。已归档为 SKILL.md.v2.2.bak
