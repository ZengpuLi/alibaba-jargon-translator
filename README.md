# Alibaba Jargon Translator Skill

把普通中文职场表达改写成「阿里味 / 大厂黑话」的 Codex Skill。

这个 Skill 适合用来润色钉钉消息、周报、OKR、述职、会议纪要，或者把一句普通话改成「赋能、抓手、闭环、对齐、拉通、沉淀、心智、体感、中台、飞轮」味道更重的表达。

## Usage

把这个仓库复制或软链接到 Codex skills 目录：

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/ZengpuLi/alibaba-jargon-translator.git ~/.codex/skills/alibaba-jargon-translator
```

然后在 Codex 里这样使用：

```text
Use $alibaba-jargon-translator 把“我今天会把接口文档写完，然后发给后端确认”改成钉钉消息版。
```

示例输出：

```text
我今天会先把接口文档版本收口并透传给后端同学，方便大家对齐字段口径和联调边界，后续基于反馈快速闭环。
```

## Modes

- `Light`: 少量黑话，适合真实工作沟通。
- `Standard`: 默认模式，适合周报、会议、述职表达。
- `Heavy`: 黑话拉满，适合玩梗和段子版表达。

支持的常见输出形态：

- 一句话版
- 钉钉消息版
- 周报版
- OKR / 述职版
- 会议纪要版
- 黑话拉满版

## What Is Included

- `SKILL.md`: Skill 触发规则、改写流程、输出风格约束。
- `references/jargon-map.md`: 公开词库、句式模板、转换规则和示例。
- `agents/openai.yaml`: Codex UI 元数据。

## Notes

这个项目基于公开网页、公开文化表述和公开流传的互联网公司黑话整理，不包含也不应包含任何阿里巴巴内部保密信息。

本项目不是阿里巴巴官方项目，也不代表阿里巴巴官方口径。真实工作场景里建议使用 `Light` 或 `Standard`，避免为了黑话而牺牲可读性。

## Public Sources

- [Alibaba Group About/Culture](https://www.alibabagroup.com/about-alibaba)
- [Alibaba Group Values Announcement](https://www.alibabagroup.com/document-1491212036011458560)
- [justjavac/ali-words](https://github.com/justjavac/ali-words)
- [互联网黑话公开整理](https://www.qianguyihao.com/post/2021-04-01-words/)

## License

MIT
