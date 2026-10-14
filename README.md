# wubowuboxiao 薄肌饮食skill

**English** | [中文](README.zh-CN.md)

A diet skill that works with **any AI: Claude, ChatGPT, Gemini, DeepSeek, Doubao, Kimi, and more**. It helps you eat for a "lean physique" (薄肌): V-taper, visible abs, clear definition without looking bulky. Use it to cut while keeping muscle, or to lean bulk.

It asks about your situation first (height, weight, goal, training, kitchen setup, foods you avoid, budget), then helps you:

- Set maintenance, cutting / bulking calories, and protein, carbs, fat
- Build a fixed daily meal structure that's easy to follow
- Read food labels, swap foods, handle hunger, and recover after eating out
- Rank supplements (core / health basics / optional / not recommended / caution) with safe upper limits
- Run weekly check-ins and adjust based on average weight, waist, and strength

> This method comes from the author's own cut, cleaned up into a general version to share. It will keep getting updated.

## How to use it (pick your AI)

The core files are [`lean-physique-diet/SKILL.md`](lean-physique-diet/SKILL.md) (English, default) and [`lean-physique-diet/SKILL.zh-CN.md`](lean-physique-diet/SKILL.zh-CN.md) (Chinese). They say the same thing. Each one is a plain instruction sheet for an AI, so you can paste either into any AI. The English version replies in whatever language you write in.

**ChatGPT**

- Best: create a GPT (Explore GPTs → Create → Configure) and paste the full SKILL.md into Instructions
- Or: create a Project and paste SKILL.md into the project instructions, or upload it as a file

**Gemini**

Create a Gem and paste the full SKILL.md into Instructions.

**Claude**

- Claude.ai / app: download the `lean-physique-diet` folder, zip it, and upload it on the Skills page in Settings
- Claude Code: put the `lean-physique-diet` folder in `~/.claude/skills/`
- Or create a Project and paste SKILL.md into the project instructions

**DeepSeek / Doubao / Kimi / Qwen / other AIs**

- If it has agents, custom assistants, or custom instructions: create one and paste the full SKILL.md
- If not: start a new chat, say "Act as my diet coach using the method below", paste the full SKILL.md, and keep chatting in that thread

> The lines between the `---` at the top are formatting info for Claude. You can delete them when pasting into other AIs, or leave them in. Either way works.

## Example prompts

Once it's set up, just talk to it:

- "I'm 175 cm, 70 kg, and want to cut until I have abs. Make me a diet plan."
- "Here's what I ate today. How much do I have left?"
- "Is this food label good for a cut?" (send a photo)
- "Here are the supplements I take. Anything doubled up or missing?"
- "My weekly average dropped 0.2 kg. Should I adjust?"

## Files

```
lean-physique-diet/
├── SKILL.md          # the skill (English, default)
└── SKILL.zh-CN.md    # Chinese version
```

## Disclaimer

This skill gives general diet and supplement information. It is not medical advice. If you're under 18, pregnant or breastfeeding, have kidney disease, diabetes, a thyroid condition, a history of eating disorders, or take prescription meds, talk to a doctor first.

## Changelog

See [CHANGELOG.md](CHANGELOG.md).

## License

MIT License. See [LICENSE](LICENSE).
