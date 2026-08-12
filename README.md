# McKee Storycraft — Claude Code Skill

## 罗伯特·麦基是谁？

**罗伯特·麦基（Robert McKee）** 是美国著名编剧导师、作家，被誉为"好莱坞编剧教父"。他的代表作《故事：材质、结构、风格和银幕剧作的原理》（*Story: Substance, Structure, Style and the Principles of Screenwriting*）是全球编剧和故事创作者的必读经典，被翻译成 20 多种语言。

麦基的核心观点是：**好故事不是靠灵感和运气，而是可以精确掌握的技艺。** 他穷尽一生研究故事的解剖结构，提炼出原理而非规则——原理告诉你"经过时间考验，这么做确实行得通"。

他的学生包括皮克斯、迪士尼的编剧团队，以及超过 60 位奥斯卡得主。无论你是写短剧、电影、小说还是短视频，麦基的故事框架都能帮你把内容做得更扣人心弦。

---

## 使用方法

### 安装

将此目录复制到 `~/.claude/skills/mckee-storycraft/`：

```bash
mkdir -p ~/.claude/skills/mckee-storycraft
cp -R . ~/.claude/skills/mckee-storycraft/
```

### 在 Claude Code 中调用

直接输入 `/mckee-storycraft` + 话题即可：

| 用法 | 示例 | 说明 |
|------|------|------|
| 不加参数 | `/mckee-storycraft` | 加载能力概览与 references 索引 |
| 按话题查询 | `/mckee-storycraft 对立原则` | 查找对应对立力量、场景设计、人物弧光等 |
| 按章节加载 | `/mckee-storycraft ch04` | 直接加载指章节（ch01–ch04） |
| 剧本诊断 | 粘贴一段剧本草稿 | 用麦基五要素做结构化体检、给出可执行改写建议 |
| 浏览目录 | `/mckee-storycraft 有哪些章节` | 查看完整章节索引 |

> 若要诊断 / 改写 / 重构剧本，Agent 会先确认类型、篇幅、目标观众、主角等最小信息，再动手。

### 核心框架速览

这个 skill 收录了麦基故事体系中最核心的思维模型：

- **原理 > 规则** — 回到艺术原理，而不是模仿范本
- **原型 > 刻板** — 发掘普世经验，用独特方式包装
- **故事是生活的隐喻** — 结构本身就是你对世界的理解
- **对立原则** — 对立力量越强，故事越吸引人
- **激励事件（触发事件）** — 彻底打破主角生活的平衡
- **场景设计** — 每个场景都是一次价值的转变
- **人物弧光** — 主角在压力下的真实改变

## Contents（文件清单）

该 skill 按标准结构组织：`SKILL.md`（调度器）+ `references/`（按需加载的知识库）。

| 文件 | 说明 |
|------|------|
| `SKILL.md` | 主 skill 调度器：能力概述、工作模式、启动协议、诊断结构、质检清单、范围边界 |
| `references/core-frameworks.md` | 十大核心框架、问题驱动索引、章节/话题索引 |
| `references/chapters/` | 四部章节深入原文（作家之道、故事元素、故事设计、写作实践） |
| `references/cheatsheet.md` | 故事原理速查表 |
| `references/glossary.md` | 麦基核心术语表（中英对照、双译名） |
| `references/patterns.md` | 可复用的故事模式与结构 |
