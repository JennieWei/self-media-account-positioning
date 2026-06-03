# Self-Media Account Positioning Skill

一个用于自媒体账号定位诊断的 Codex Skill。

它的角色不是表单收集器，而是一个账号定位专家：通过阶段式提问、概念解释、专业判断和纠偏，帮助用户从模糊的账号想法，逐步推导出可开拍、可验证、可迭代的账号定位。

## 使用场景

适合在这些情况下使用：

- 准备从零开始做一个自媒体账号
- 已经有账号，但定位混乱、流量不稳定或内容方向不清晰
- 想重新设计账号人设、目标用户、内容价值和竞争优势
- 不知道自己适合口播、录屏、案例拆解、生活场景还是其他表达方式
- 想把账号定位落到具体选题，而不是只写一段漂亮简介

## 核心流程

Skill 会按照这个顺序一步步推进：

```text
价值 -> 用户 -> 关系 -> 人设 -> 竞争优势 -> 类型/风格 -> 选题验证
```

它不会一次性向用户丢出很多问题，而是每轮只问一个核心问题。用户回答后，Skill 会先做专家判断，再决定是追问、纠偏，还是进入下一阶段。

## 主要能力

- 解释账号定位中的关键概念，并给出短案例
- 识别用户回答里的模糊、风险和不现实之处
- 帮用户把泛泛的人群压缩成具体用户画像
- 判断创作者和用户之间应该建立什么关系
- 挖掘可被观众记住的人设营销点
- 用「正、反、和、跨、借、弱」框架寻找竞争优势
- 通过能力和场景诊断表达方式，而不是让用户凭空选择形式
- 在用户想不出选题时，先生成候选选题，再判断可执行性

## 安装位置

将仓库中的 `self-media-account-positioning/` 目录放入 Codex skills 目录：

```text
~/.codex/skills/self-media-account-positioning
```

重启 Codex 后即可调用。

## 调用示例

```text
Use $self-media-account-positioning to guide me step by step through designing a self-media account positioning.
```

中文也可以：

```text
Use $self-media-account-positioning 帮我一步步诊断并设计一个自媒体账号定位
```

## 输出形式

当信息足够后，Skill 会输出：

- 专家诊断
- 一句话账号定位
- 目标用户
- 核心价值
- 创作者和用户的关系
- 人设印象
- 竞争优势
- 类型和风格建议
- 高 / 中 / 低三个定位版本
- 选题验证
- 最建议启动的版本和下一步行动

## 目录结构

```text
self-media-account-positioning/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── output-template.md
    └── question-bank.md
```
