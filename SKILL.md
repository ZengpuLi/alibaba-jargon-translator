---
name: alibaba-jargon-translator
description: Transform ordinary Chinese workplace text into Alibaba-style and Chinese internet-company jargon. Use when the user asks for 阿里黑话, 阿里味, 大厂黑话, 互联网黑话, 周报/月报/OKR/述职/会议话术 polishing, or converting plain Chinese into terms such as 赋能, 抓手, 闭环, 对齐, 拉通, 沉淀, 心智, 体感, 中台, 业务链路, 复盘, and 飞轮.
---

# Alibaba Jargon Translator

## Core Use

Rewrite ordinary Chinese into Alibaba-style workplace language using public, generic "阿里味/大厂黑话" patterns. Keep the result useful by default, and increase density only when the user asks for "浓一点", "黑话拉满", "段子版", or "纯阿里味".

When converting text, read `references/jargon-map.md` for the term map, sentence templates, and examples.

## Default Workflow

1. Identify the intent, audience, and artifact:
   - chat reply, DingTalk-style update, weekly report, OKR, meeting notes, review, escalation, self-introduction, resume bullet, or playful meme.
2. Pick a jargon density:
   - **Light**: 20-30% jargon. Suitable for real work messages.
   - **Standard**: 40-55% jargon. Suitable for Alibaba-style reports and meetings.
   - **Heavy**: 70%+ jargon. Suitable for jokes, parody, or deliberate "黑话拉满".
3. Preserve factual meaning. Do not invent metrics, ownership, deadlines, or internal facts.
4. Apply Alibaba/internet-company style moves:
   - Turn tasks into "抓手", "动作", "打法", "路径".
   - Turn problems into "痛点", "卡点", "风险点", "机会点".
   - Turn collaboration into "对齐", "拉通", "共创", "协同", "透传".
   - Turn completion into "闭环", "收口", "落地", "沉淀", "复盘".
   - Turn impact into "业务价值", "用户心智", "履约体感", "规模化收益".
5. Output only the rewritten text unless the user asks for explanation, comparison, or a glossary.

## Style Rules

- Prefer concise, credible phrases over piling up buzzwords.
- Use "同学" for colleagues when natural, but do not force it into every sentence.
- Use Alibaba culture phrases only when they fit the context: "客户第一", "因为信任, 所以简单", "此时此刻, 非我莫属", "今天最好的表现是明天最低的要求".
- Keep sensitive or confidential content out. If the user provides internal-only terms, rewrite around them without expanding or exposing private meaning.
- Do not claim the wording is official Alibaba wording. Treat this as a public-style parody/workplace writing aid.
- For real workplace writing, avoid sarcasm and keep the final version readable.

## Output Modes

If the user does not specify a mode, use **Standard**.

- **一句话版**: Produce one polished sentence.
- **钉钉消息版**: Short, action-oriented, friendly.
- **周报版**: Use "本周进展/问题风险/下周计划" structure if the input contains multiple points.
- **OKR/述职版**: Emphasize objective, measurable result, strategy, owner, and next step.
- **会议纪要版**: Use "背景/结论/Action/Owner/Deadline/风险" structure.
- **黑话拉满版**: Allow playful high-density jargon while preserving the original meaning.

## Quick Pattern

For a simple sentence, use this mental template:

`围绕 [目标/场景], 通过 [抓手/动作] 拉通 [协作方/资源], 对齐 [标准/预期], 推动 [结果] 闭环, 并沉淀为 [方法论/机制/资产].`

For a status update:

`当前 [事项] 已完成 [进度/结果], 核心卡点在 [风险/依赖]. 下一步会以 [动作] 为抓手, 拉齐 [相关方], 在 [时间] 前完成闭环.`

## Examples

Plain: `我明天把文档发给你。`

Standard: `我明天先把文档版本透传出来, 方便大家对齐上下文, 后续基于反馈快速收口。`

Plain: `这个功能还没做完, 需要产品确认需求。`

Standard: `当前功能链路还在推进中, 主要卡点是需求口径需要和产品同学再拉齐。需求确认后我会推动开发动作闭环。`

Plain: `我们要提高用户留存。`

Heavy: `围绕用户留存这个核心北极星指标, 需要从用户心智、使用链路和履约体感三个维度拆解抓手, 通过精细化运营和产品机制迭代形成增长飞轮。`
