# 花生十三 · 行测三件套 Skill（huasheng13-sanhaojian）

把花生十三 / 四海公考 2026 系统班的**三个行测模块**方法论整合进一个统一入口 skill，便于按需调用，不再切换多个 skill。

## 覆盖模块

| 模块 | 来源 | 能力卡 | 入口 |
| --- | --- | --- | --- |
| 资料分析 | 27 视频蒸馏 | 11 张 | `references/ziliao/_index.md` |
| 判断推理 | 16 讲蒸馏 | 6 张 | `references/panduan/_index.md` |
| 言语理解 | 系统课蒸馏 | 15 张 + 速查表 | `references/yanyu/_index.md` |

## 目录结构

```
huasheng13-sanhaojian/
├── SKILL.md                # 总入口：模块识别 + 路由
├── README.md
├── LICENSE
└── references/
    ├── ziliao/             # 资料分析
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
    ├── panduan/            # 判断推理
    │   ├── _index.md
    │   ├── tixingfenlei.md
    │   ├── guiyin-lunzheng.md
    │   ├── sanquantishi.md
    │   ├── zhijie-genben-yuanyin.md
    │   ├── yiban-zhiyi.md
    │   └── dingyiti.md
    └── yanyu/              # 言语理解
        ├── _index.md       # 模块导航（15 能力路由表）
        ├── overview.md
        ├── glossary.md
        ├── cheatsheet.md
        ├── capability-index.md
        ├── capabilities/   # 15 张能力卡
        └── extras/cheatsheet-print.html
```

## 使用方法

1. 把本目录放到 `~/.workbuddy/skills/` 下即可被 WorkBuddy 识别。
2. 问行测题时，本 skill 会先判断属于「资料 / 判断 / 言语」哪一模块，再进入对应 `_index.md` 与具体能力卡。

## 说明

- 本 skill 整合自 `sihai-ziliao-skill`、`sihai-panduan-skill`、`huasheng13-yanyu` 三个独立 skill；`gongkao-huasheng13`（含数量/申论等）未纳入。
- 数量关系、常识判断、申论不在本三件套覆盖范围内。
- 版权归花生十三 / 四海公考所有，本仓库仅作个人学习笔记，详见 `LICENSE`。
- 版本：2026-10-28 整合封版。
