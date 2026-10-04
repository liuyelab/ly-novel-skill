---
name: ultimate-novel-benchmark
description: "Select, verify, compare, and synthesize multiple Chinese novels into a project-specific writing baseline. Use when opening or redirecting a novel project, changing platform or genre, refreshing stale guidance, comparing several supplied or accessible works, or preparing reusable craft rules before substantial outlining, drafting, continuation, or revision. Use long-analyze or short-analyze for close reading of one work."
---

# 对标样本与写作基线

用最少但足够的高匹配样本建立可重复读取的项目基线。样本用于理解为什么读者点开、继续和获得兑现，不用于拼接原文、模仿某位作者的独特表达或改变本书正史。

选样、比较和形成建议前完整读取 [小说质量核心](../ultimate-novel/references/reader-experience-first.md)。不加载人物行动、正文场景和章名等详细规则。项目存在 `追踪/项目经验.md` 时先读取，其中经数据或作者验证的做法优先于新样本推测。

## 是否需要样本

- 项目已有有效基线且本轮没有方向变化：0 本，直接复用；
- 定点校准文气、开篇或单一问题：通常 1 至 2 本；
- 新项目、换平台或换题材：通常 2 至 6 本；
- 方向高度不确定且样本差异确有分析价值：最多扩至 10 本。

数量不是配额。作者提供多少先使用多少；证据不足时说明，不为凑数选低相关作品。

## 选样

优先判断：

1. 是否匹配目标读者和本项目承诺；
2. 是否能解释点击、持续阅读和兑现；
3. 是否有足够可读正文或可核验证据；
4. 是否提供本项目当前缺少的具体能力；
5. 多个样本能否形成互补，而非同质重复。

文学地位、作者名气、榜单位置、道德正确和流程完整不能单独证明好看。当前评分、在读和榜单属于时间快照，不直接证明收入、追读或长期成功。

记录平台、题材、可读范围、缺章、版本、数据时间和证据限制。作者已下载样本时优先使用本地可读文本；只可见简介或片段时降低结论强度，不假装读完整书。

## 分析分工

单部长篇或指定章节交给 `ultimate-novel-long-analyze`；单篇短篇交给 `ultimate-novel-short-analyze`。本模块只负责样本选择、覆盖检查、横向比较和项目综合，不复制逐本拆解流程。

比较时区分：

- 多个样本共同支持的方法；
- 某位作者的个人选择；
- 只在特定题材、视角、篇幅或平台成立的条件；
- 与本项目正史和作者气质冲突、不能迁移的部分。

## 项目基线

输出最小充分字段：

```markdown
# 项目写作基线

## 目标读者与作品承诺
## 点击理由、持续阅读引擎、兑现节奏与余味
## 样本分工、正文范围与证据边界
## 可迁移的结构、场景、人物、对白和情绪方法
## 禁止照搬及本项目不适用项
## 开写前最小检查与未确认项
```

每条方法说明读者效果、样本证据、适用条件和写坏风险。基线只管“怎样写”；作者决定与正史管“写什么”。冲突时作者和正史优先，不能用样本覆盖人物、事实和结局。

## 停靠

作者只要求基线时完成后停止。方向尚未确认时不自动写正式大纲；作者确认并要求继续时才进入相应写作模块。
