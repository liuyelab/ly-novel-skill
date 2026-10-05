---
name: ultimate-novel
description: "Route broad, ambiguous, or multi-stage Chinese novel requests across market evidence, topic selection, benchmark baselines, analysis, setup, import, outlining, drafting, review, revision, packaging, and performance diagnosis. Use when several stages are combined, the correct specialized module is unclear, or a brief contextual follow-up must inherit the current stage; skip this router when one ultimate-novel-* skill clearly matches."
---

# 天道小说Skill 路由

本模块只选择专业模块和处理顺序，不自行评价、创作或修改作品，也不加载正文细则。能够确定目标模块时直接进入，不先加载本路由。

## 每轮调用

“继续”“可以”“按这个改”“接着写”等简短指令继承当前小说任务阶段，但每个用户回合仍重新读取对应专业模块。目标模块无法读取时说明阻断，不绕过 Skill 直接处理。

## 路由表

| 作者意图 | 加载模块 |
|---|---|
| 初始化或补齐小说项目 | `ultimate-novel-setup` |
| 获取榜单、后台或市场证据 | `ultimate-novel-market-data` |
| 筛选多部对标并建立项目写作基线 | `ultimate-novel-benchmark` |
| 长篇选题、方向比较和市场验证 | `ultimate-novel-long-scan` |
| 拆解一部长篇、指定章节或黄金三章 | `ultimate-novel-long-analyze` |
| 长篇设定、大纲、细纲、正文、续写、返修和暗线推演 | `ultimate-novel-long-write` |
| 短篇选题、方向比较和市场验证 | `ultimate-novel-short-scan` |
| 拆解单篇或少量指定短篇 | `ultimate-novel-short-analyze` |
| 构思、写作、续写或修改短篇 | `ultimate-novel-short-write` |
| 导入已有小说并准备维护或续写 | `ultimate-novel-import` |
| 审查好看程度、逻辑、事实、人物和表达 | `ultimate-novel-review` |
| 去 AI 味、修对白、叙述和模板感 | `ultimate-novel-deslop` |
| 书名、简介、封面和发布包装 | `ultimate-novel-cover` |
| 点击、追读、完读、转化和章节流失复盘 | `ultimate-novel-performance-review` |

## 多阶段顺序

1. 数据先于市场判断；
2. 选题先于对标基线和正式写作；
3. 导入与正史核对先于续写；
4. 结构、事实和人物问题先于表达润色；
5. 正文先形成草稿，正式提交前再独立审稿；
6. 包装必须来自正文真实承诺，发布数据诊断后再路由到相应返修模块。

只加载当前最早阻塞环节。完成当前请求后停止，不自动跨入会改变作品方向的下一阶段。

## 作者裁决

最终选题、核心卖点、主角长期目标、读者承诺、黄金三章整体方向、重大候选未来、推翻正史、弃书重开和整体换线由作者决定。普通执行、定点修正和无阻断续写不反复确认。

## 不明确时

先用现有上下文判断。只有两个入口同样可能且选错会产生明显不同结果时，才问一个短问题，不发长表单。
