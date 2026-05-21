# 雅思 6.5 备考 · 第一阶段 W1-W12 基础重建

> **目标**:6 个月内雅思 6.5 · 第一阶段(W1-W12)打基础,第二阶段(W13-W24)冲刺应试
> **当前水平**:中等(底子在但已退化,写作有基础语法漏洞、口语短句行长句崩)
> **时间预算**:30-60 分钟/天 · 混合时间
> **生成日期**:2026-05-25

---

## 这份计划是怎么设计的

这是一份给"底子在但久没用"的人设计的计划。直接冲雅思 6.5 是吃力的——必须先补一段"基础重建"(语法 + 词汇),再上应试技巧效率才高。所以这第一阶段聚焦语法重建、高频词扩充、听力打底、写作 Task 1 入门。时间紧,每分钟都要用在刀刃上,没有"看美剧学英语"这种低效内容。

## 12 周路径概览

| 主题 | 周次 | 目标 |
|---|---|---|
| 语法重建 · 时态/单复数/冠词 | W1-W2 | 补写作里最容易出错的三个基础点 |
| 语法重建 · 从句/长句结构 | W3-W4 | 解决"短句行长句崩"问题 |
| 高频词第一轮 · 1500 词 | W5-W6 | 词汇是 6.5 的硬门槛 |
| 听力精听突破 | W7-W8 | 进入雅思 Section 3-4 难度 |
| 写作 Task 1 入门 | W9-W10 | 图表描述题先拿下 |
| 第一次模考 + 复盘 | W11-W12 | 决定第二阶段重点 |

## 每日 45 分钟分配

- **听力精听 15 min** — 雅思 Section 1-2 真题
- **跟读模仿 10 min** — 1-2 分钟原音模仿
- **语法+写作 15 min** — 一个语法点 + 一段写作 + AI rewrite
- **词汇阅读 5 min** — 雅思核心词

完成 3 项算打卡。

## 推荐资源

- 语法书:*English Grammar in Use*(Raymond Murphy 蓝皮书,京东可买)
- 听力:Cambridge IELTS 11-18 真题(淘宝/微信小店)
- 词汇:王陆雅思王听力词汇,或《雅思核心词汇 21 天突破》
- 写作反馈:Claude / ChatGPT,prompt 用 "Rewrite as a native English speaker would, then list top 3 differences"
- BBC 6 Minute English(官网或小宇宙)

## 检验机制

- **W4**:语法基础测试(Grammar in Use 章节末)
- **W8**:雅思听力一套(看是否到 5.5 段)
- **W12**:完整模考 + 决定第二阶段

## 下周一开始之前

1. 京东买《English Grammar in Use》中级蓝皮书
2. 淘宝下单 Cambridge IELTS 11-14 真题音频

---

## 追踪器配置(给工具用,不用读)

```json
{
    "title": "雅思 6.5 备考 · 第一阶段",
    "subtitle": "30-60 分钟/天 · 完成 3 项及以上算打卡",
    "startDate": "2026-05-25",
    "storageKey": "ielts-6-5-phase-1",
    "dailyTasks": [
        { "id": "listen", "name": "听力精听", "detail": "15 分钟 · 雅思 Section 1-2 真题", "icon": "ti-headphones", "color": "#378add" },
        { "id": "shadow", "name": "跟读模仿", "detail": "10 分钟 · 1-2 分钟原音模仿 + 录音对比", "icon": "ti-microphone", "color": "#1D9E75" },
        { "id": "grammar", "name": "语法+写作", "detail": "15 分钟 · 1 个语法点 + 1 段写作 + AI rewrite", "icon": "ti-pencil", "color": "#D85A30" },
        { "id": "vocab", "name": "词汇阅读", "detail": "10 分钟 · 雅思核心词 + 短文精读", "icon": "ti-vocabulary", "color": "#7F77DD" }
    ],
    "checkInThreshold": 3,
    "themes": [
        {
            "weeks": 2,
            "title": "语法重建 · 时态/单复数/冠词",
            "description": "补写作里最容易出错的三个基础点",
            "color": "#EEEDFE", "textColor": "#3C3489",
            "content": {
                "listen": "Cambridge IELTS 11 · Test 1 Section 1-2 精听",
                "shadow": "BBC 6 Minute English 选一集跟读到耳熟",
                "grammar": "Grammar in Use Unit 1-14(时态)· 每天 1 单元",
                "vocab": "雅思核心词第 1-2 章 · 每天 20 词 + 例句"
            }
        },
        {
            "weeks": 2,
            "title": "语法重建 · 从句和长句结构",
            "description": "解决'短句行长句崩'· 学会写复合句",
            "color": "#E1F5EE", "textColor": "#085041",
            "content": {
                "listen": "Cambridge IELTS 11 · Test 2 Section 1-2 精听",
                "shadow": "TED-Ed 短视频(5 分钟内)· 一集跟读 3 遍",
                "grammar": "Grammar in Use Unit 90-110(从句)· 每天写 3 个长句",
                "vocab": "雅思核心词第 3-4 章 · 每天 20 词"
            }
        },
        {
            "weeks": 2,
            "title": "高频词第一轮 · 1500 词",
            "description": "词汇是 6.5 的硬门槛 · 这两周冲刺第一遍",
            "color": "#FAECE7", "textColor": "#712B13",
            "content": {
                "listen": "Cambridge IELTS 12 · Test 1 Section 1-2 精听",
                "shadow": "BBC Learning English Podcast 一集 · 跟读重点段",
                "grammar": "Grammar in Use 巩固复习 · 每天写一段含新词的话",
                "vocab": "雅思核心词第 5-8 章 · 每天 50 词(第一轮要快)"
            }
        },
        {
            "weeks": 2,
            "title": "听力精听突破",
            "description": "把 6 Minute 听到 90%+ · 进入 Section 3 难度",
            "color": "#FBEAF0", "textColor": "#72243E",
            "content": {
                "listen": "Cambridge IELTS 12 · Test 2 Section 3-4(进入难段)",
                "shadow": "TED 演讲(10 分钟以内)选段跟读",
                "grammar": "雅思 Task 1 图表描述结构 · 每天 100 字图表",
                "vocab": "雅思核心词第 9-12 章 + 听力高频词"
            }
        },
        {
            "weeks": 2,
            "title": "写作 Task 1 入门",
            "description": "图表描述题对 IT 背景人相对友好 · 先拿下",
            "color": "#FAEEDA", "textColor": "#633806",
            "content": {
                "listen": "Cambridge IELTS 13 · Test 1 整套听力",
                "shadow": "雅思口语 Part 2 范例跟读",
                "grammar": "Task 1 完整范文研读 + 仿写 · 每天 1 篇 150 字",
                "vocab": "Task 1 高频表达(increase/decrease 同义替换 30 组)"
            }
        },
        {
            "weeks": 2,
            "title": "第一次完整模考 + 复盘",
            "description": "全面诊断当前水平 · 决定第二阶段重点",
            "color": "#F1EFE8", "textColor": "#444441",
            "content": {
                "listen": "Cambridge IELTS 14 · 完整模考 1 套(限时)",
                "shadow": "口语 Part 1+2+3 自己答 + 录音对比",
                "grammar": "Task 2 议论文初步尝试 · 每天写 1 段",
                "vocab": "复习前 12 章高频词 · 错词重点突破"
            }
        }
    ],
    "checkpoints": [
        { "week": 4, "text": "语法基础自测(Grammar in Use 章节末)" },
        { "week": 8, "text": "听力阶段测试 · 看是否到雅思 5.5" },
        { "week": 12, "text": "完整模考 · 决定进入第二阶段" }
    ]
}
```
