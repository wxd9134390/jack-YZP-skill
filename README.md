# 花生十三 · 行测三件套（资料分析 + 判断推理 + 言语理解）

> 把花生十三 / 四海公考 2026 系统班的三个行测模块方法论，整合进**一个**统一 skill 入口，告别在多个 skill 间切换。

## 这是什么

| 模块 | 来源 | 能力卡 | 拆分版仓库（单模块） |
| --- | --- | --- | --- |
| 资料分析 | 27 视频蒸馏 | 11 张 | [jack-ziliao-skill](https://github.com/wxd9134390/jack-ziliao-skill) |
| 判断推理 | 16 讲蒸馏 | 6 张 | [jack-panduan-skill](https://github.com/wxd9134390/jack-panduan-skill) |
| 言语理解 | 系统课蒸馏 | 15 张 + 速查表 | [jack-Yanyu-skill](https://github.com/wxd9134390/jack-Yanyu-skill) |

本仓库是三者的**整合版**，适合想一次装好、按需调用全部行测方法论的用户。三个拆分版仓库仍保留，方便只想用单模块的人。

## 目录结构

```
huasheng13-sanhaojian/
├── SKILL.md                # 总入口：模块识别 + 路由
├── README.md
├── LICENSE
└── references/
    ├── ziliao/             # 资料分析（11 卡 + _index 导航）
    │   ├── _index.md       # 模块导航（11 能力 + 卡索引）
    │   ├── abrx-core.md
    │   ├── susuan-shuxing.md
    │   ├── zengsu-bijiao.md
    │   ├── jiangfu-jueduizhi.md
    │   ├── ziliao-yuanze.md
    │   ├── beishu-pingjunshu.md
    │   ├── ronghe-zonghe.md
    │   ├── bijiao-lei.md
    │   ├── xuexifa-duanxianfa.md
    │   ├── yunju-zengzhang.md
    │   └── yicuo-koujue.md
    ├── panduan/            # 判断推理（6 卡 + _index 导航）
    │   ├── _index.md
    │   ├── tixingfenlei.md
    │   ├── guiyin-lunzheng.md
    │   ├── sanquantishi.md
    │   ├── zhijie-genben-yuanyin.md
    │   ├── yiban-zhiyi.md
    │   └── dingyiti.md
    └── yanyu/              # 言语理解（15 卡 + 速查表）
        ├── _index.md       # 模块导航（15 能力路由表）
        ├── overview.md
        ├── glossary.md
        ├── cheatsheet.md
        ├── capability-index.md
        ├── capabilities/    # 15 张能力卡
        └── extras/cheatsheet-print.html
```

## 如何安装使用

1. 把本仓库克隆 / 下载到本地 WorkBuddy 的 skills 目录：
   ```bash
   # 放到用户级 skills（全局可用）
   git clone https://github.com/wxd9134390/jack-YZP-skill.git ~/.workbuddy/skills/huasheng13-sanhaojian
   ```
2. 在 WorkBuddy 里直接问行测题（如「这道题增长率怎么算」「逻辑填空怎么找对应」），skill 会先判断属于「资料 / 判断 / 言语」哪一模块，再进入对应 `references/<模块>/_index.md` 与具体能力卡作答。

## 三大模块方法论速览

### 资料分析
- **ABRX 四量**：A=基期，B=现期，X=增长量，R=增长率；知二求二。
- **速算决策**：负 / 0–10% → 化除为乘；0–20% → 假设分配；接近常用分数 → 415 分数法；>20% → 直算。
- **增速三问**：多少/大小 → 增长量 X；快慢/增幅 → 增长率 R（带符号）；变化幅度 → |R|。
- **高频考点**：百分点=差值；翻 N 番=2^N；降幅=|R|（仅 R<0）；比重差可秒杀、比值差不可秒杀。
- **年均增长量**：(末期−基期)/N，N=末期−基期年份（算出来）；格尺法锚点 1.1⁴=1.46 / 1.2⁴=2.07。

### 判断推理
- **题型三分**：论证类（归因/质疑/支持）、推出类（必然性推理）、分析类（匹配/排序）。
- **归因质疑力度**：另有他因(弱) < 因果倒置(强) ≈ 否定此因(强)。
- **三圈质疑**：同因异果、异因同果、无因有果；四圈补全对比实验。
- **直接根本原因**：支持谁 → 让谁是根本原因；质疑谁 → 让谁是直接原因。
- **一般质疑三段攻击**：推理漏洞 > 结论无中生有 > 论据有误。
- **定义题**：先抓被定义词（最典型特征），反对机械字面匹配。

### 言语理解
- **先判文段类型再谈内容**：说理类盯一句主旨（对策在首/尾，找核心做法）；科普类求概括全面（允许上位词，忌片面）；新闻类只抓「新」（专名不抽象）。
- **错误选项穷举**：出处有误 / 客观表达(说理) / 拼好句 / 无核心做法·片面(科普) / 无新(新闻)。
- **六题型共一套判据**：标题=主旨变形，下文推断=结构续写，语句填入=缺块反推，语句排序=结构复位。
- **逻辑填空**：先句内找逻辑对应（因果/比喻/近反义/褒贬/用词一致），再用五维辨析定词。

## 覆盖边界

- ✅ 覆盖：资料分析、判断推理、言语理解（行测三大模块）。
- ❌ 不覆盖：数量关系、常识判断、申论、面试（如需见 `gongkao-huasheng13` 或专项 skill）。

## 来源与版权

- 资料分析：四海公考 / 花生十三（鹏鹏老师）2026 系统班「资料分析」27 视频蒸馏。
- 判断推理：四海公考 / 花生十三（黄老师）2026 系统班「判断推理」16 讲蒸馏。
- 言语理解：花生十三 2026 言语理解系统课蒸馏。
- 版权：课程版权归原作者所有，本仓库仅作个人学习笔记，详见 `LICENSE`。
- 版本：2026-10-28 整合封版。

---

> 配套：本仓库同时已存入 WorkBuddy 个人资料库，可作为可检索的知识沉淀使用。
