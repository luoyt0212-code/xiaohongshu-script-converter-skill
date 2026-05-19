---
name: xiaohongshu-script-converter
description: Convert Chinese spoken-video scripts into concise Xiaohongshu/RedNote posts with titles, structure, captions, hashtags, and image prompts.
---

# 口播脚本转小红书文案

Use this skill when the user provides a Chinese spoken-video script, transcript, rough notes, or long-form talking points and wants to turn it into a Xiaohongshu/RedNote-ready post.

## Core Job

Transform verbose spoken language into polished Xiaohongshu content:

1. Extract the strongest central idea.
2. Remove filler, repetition, and loose transitions.
3. Rebuild the piece as a readable image-text post.
4. Generate multiple title options.
5. Provide image or carousel prompts.
6. Keep the author's expertise and personality visible.

## Input You Should Ask For

If the user gives enough source material, start directly.

If the input is too thin, ask for one of these:

- The original spoken script or transcript.
- The intended audience.
- The desired tone: professional, sharp, warm, contrarian, beginner-friendly, or investor-style.
- Whether the output is for Xiaohongshu, WeChat Channels, Douyin captions, or a mixed workflow.

## Conversion Principles

Spoken scripts are usually loose, repetitive, and context-heavy. Xiaohongshu posts need a clearer promise and denser information.

Follow these principles:

- Keep the user's real judgment. Do not turn sharp insight into generic encouragement.
- Compress repeated sentences into one stronger sentence.
- Replace abstract claims with concrete examples, scenes, or contrasts.
- Preserve useful personal positioning, especially professional experience, investment judgment, founder lessons, and AI transformation observations.
- Avoid exaggerated self-praise. Professional credibility should come from the reasoning, not from saying "I am professional."
- Make the hook understandable in the first 3 seconds.
- Use short paragraphs and strong line breaks.
- Do not fabricate facts, data, people, or cases.

## Output Format

Return the result in this structure:

```markdown
## 1. 核心提炼

- 核心观点：
- 适合人群：
- 内容角度：

## 2. 标题备选

1. ...
2. ...
3. ...
4. ...
5. ...

## 3. 小红书正文

...

## 4. 配图建议

### 封面图
- 画面：
- 封面文字：

### 轮播图结构
1. ...
2. ...
3. ...
4. ...
5. ...

## 5. 标签

#标签1 #标签2 #标签3

## 6. 可选改写方向

- 更专业版：
- 更口语版：
- 更反常识版：
```

## Title Patterns

Use title patterns such as:

- "很多人以为 X，其实真正的问题是 Y"
- "我看了很多 X，发现最容易被忽略的是 Y"
- "别急着做 X，先想清楚 Y"
- "一个投资人视角下的 X 判断"
- "X 不是能力问题，而是系统问题"

Avoid empty titles such as:

- "分享一些思考"
- "我的一点感悟"
- "关于某某的看法"
- "普通人一定要知道"

## Body Pattern

For most posts, use this rhythm:

1. Hook: one sharp contradiction or real scene.
2. Context: why this matters now.
3. Main insight: 2-4 points with clear logic.
4. Example: one concrete case or analogy.
5. Takeaway: what the reader can do next.

## Image Prompt Pattern

When generating image prompts, keep them platform-native:

- Clean Chinese editorial poster.
- Clear cover text area.
- Not too many elements.
- Professional but approachable.
- Prefer real-life work scenes, diagrams, notebooks, meeting rooms, devices, charts, or simple symbolic compositions.

Example:

```text
一张适合小红书封面的中文知识型海报，主题是“AI转型不是买工具，而是重做流程”。画面是一个投资人视角的工作桌面：笔记本电脑、会议纪要、流程图、咖啡杯，整体干净、有专业感，留出上方大标题区域，中文字体清晰，现代商业杂志风格。
```

## Quality Checklist

Before finalizing, check:

- Is the first line strong enough to stop scrolling?
- Did you remove spoken filler?
- Is there at least one concrete example or contrast?
- Does the post sound like a real person with judgment?
- Are the image prompts usable by an image model?
- Are the tags specific enough for discovery?

## Source Note

This open-source skill was prepared from the public overview of the YouMind skill "口播脚本转小红书文案V2.0". The original YouMind instructions were private at the time this repository was prepared, so this is an independently structured shareable version rather than an exact export of the private prompt.
