# wubowuboxiao 薄肌饮食skill

[English](README.md) | **中文**

一个通用的 AI 饮食 skill，**Claude、ChatGPT、Gemini、DeepSeek、豆包、Kimi 等都能用**。帮你按「薄肌」目标（倒三角、腹肌清楚、线条明显但不臃肿）做减脂保肌或干净增肌的饮食计划。

它会先问清楚你的情况（身高体重、目标、训练量、厨具、忌口、预算），再帮你：

- 算维持热量、减脂/增肌热量和蛋白质、碳水、脂肪
- 搭一套固定好执行的每日饮食结构
- 看食品标签、给替换方案、饿了怎么加餐、外食之后怎么办
- 补剂分级推荐（核心 / 健康基础 / 可选 / 不推荐 / 谨慎），附安全上限
- 每周复盘，按体重周平均、腰围、力量变化来微调

> 这套方法来自作者自己的减脂实践，整理成通用版本分享出来，会持续更新。

## 怎么用（选你用的 AI）

核心文件：[`lean-physique-diet/SKILL.md`](lean-physique-diet/SKILL.md)（英文版，默认）和 [`lean-physique-diet/SKILL.zh-CN.md`](lean-physique-diet/SKILL.zh-CN.md)（中文版）。两份内容一样，就是写给 AI 的说明书，复制任意一份进任何 AI 都能用。英文版也会自动用你说话的语言回复。

**ChatGPT**

- 推荐：新建一个 GPT（Explore GPTs → Create → Configure），把 SKILL.md（或中文版）全文粘贴到 Instructions 里
- 或者：新建一个 Project，把 SKILL.md 粘贴到项目指令里，或者作为文件上传

**Gemini**

新建一个 Gem，把 SKILL.md（或中文版）全文粘贴到 Instructions 里。

**Claude**

- Claude.ai / App：下载 `lean-physique-diet` 文件夹，打包成 zip，在设置的 Skills（技能）页面上传
- Claude Code：把 `lean-physique-diet` 文件夹放到 `~/.claude/skills/` 下面
- 也可以新建一个 Project，把 SKILL.md 粘贴到项目指令里

**DeepSeek / 豆包 / Kimi / 通义 / 其他 AI**

- 有「智能体 / 自定义助手 / 自定义指令」功能的：新建一个，把 SKILL.md（或中文版）全文粘贴进去
- 没有的：新开一个对话，第一句发「请按下面这份方法当我的饮食教练」，再把 SKILL.md（或中文版）全文贴进去，之后都在这个对话里聊

> 开头 `---` 之间那几行是 Claude 用的格式信息，粘贴到其他 AI 时可以删掉，留着也没影响。

## 用法举例

设置好之后，直接跟 AI 说，比如：

- 「我 175 cm，70 kg，想减脂到有腹肌，帮我做个饮食计划」
- 「这是我今天吃的，帮我算算还剩多少」
- 「这个食品标签适合减脂吗？」（发图片）
- 「我现在吃这些补剂，有没有重复或者缺的？」
- 「这周体重平均降了 0.2，要不要调整？」

## 文件结构

```
lean-physique-diet/
├── SKILL.md          # skill 本体（英文，默认）
└── SKILL.zh-CN.md    # 中文版
```

## 免责声明

本 skill 只提供一般性的饮食和补剂信息，不是医疗建议。未成年人、孕期或哺乳期、有肾病、糖尿病、甲状腺疾病、饮食障碍史或正在服用处方药的人，请先咨询医生。

## 更新记录

见 [CHANGELOG.md](CHANGELOG.md)。

## 协议

MIT License，见 [LICENSE](LICENSE)。
