# Game Translation with Claude Code

用 Claude Code 翻译游戏/应用的完整指南。从实战中提炼，解决 AI 翻译"不说人话"的问题。

> Translate games/apps with Claude Code. Battle-tested guide that fixes the "doesn't sound human" problem in AI translation.

---

## 这是什么

一份操作指南（Skill），教你用 [Claude Code](https://docs.anthropic.com/en/docs/claude-code) 把英文游戏翻译成中文。

包含：
- **完整操作步骤**：从复制副本到配置字体到并行翻译
- **说人话翻译指南**：AI 翻译的典型问题和修复方法
- **反面案例对照表**：错误翻译 vs 正确翻译，附问题分析
- **常见坑速查**：中文引号语法错误、字体方框、界面崩溃等

---

## 快速开始

### 方法一：作为 Claude Code 项目指令使用

1. 把 `CLAUDE.md` 放到你的项目根目录
2. 把 `translation-guide.md` 放到项目根目录
3. 启动 Claude Code，告诉它翻译你的游戏

```bash
# 在游戏所在目录
cp /path/to/this/repo/CLAUDE.md .
cp /path/to/this/repo/translation-guide.md .
claude
```

然后对 Claude 说：
```
把这个游戏翻译成中文，参考 translation-guide.md 的步骤和翻译原则
```

### 方法二：手动参考

直接阅读 `translation-guide.md`，按步骤操作。

---

## 文件说明

| 文件 | 用途 |
|-----|------|
| `CLAUDE.md` | Claude Code 项目指令，让 Claude 自动遵循翻译原则 |
| `translation-guide.md` | 完整翻译指南（操作步骤 + 说人话原则 + 反面案例） |

---

## 适用范围

已验证：
- **Ren'Py 视觉小说**（.rpy 文件）

理论适用：
- Electron 应用（.json / .html）
- Unity 游戏（本地化文件）
- 任何包含文本文件的应用

---

## 核心原则预览

### 说人话翻译四条铁律

1. **骂人的词就翻成骂人的词** — AI 天然保守，会把 "fuck" 翻成 "该死"。不要替原文文明化
2. **口语用短句** — 真人说话不用从句
3. **情绪词优先于精确词** — 人在情绪中挑最顺嘴的词，不是最精确的
4. **语调跟随场所切换** — 同一作品里，街头骂战和学术演讲用不同的腔

### AI 翻译的典型病

| 症状 | 表现 | 治疗 |
|-----|------|------|
| 论文腔 | "达到了极限" | 换口语：零、压根 |
| 逻辑腔 | "如果A那么B" | 断成短句 |
| 中性腔 | 所有角色一个温度 | 先判断角色性格 |
| 含蓄病 | "吸我" | 补具体宾语 |
| 发挥病 | 添加原文没有的 | 对照原文删多余的 |

更多内容见 `translation-guide.md`。

---

## 来源

从 DEBTORS 6.0（Ren'Py 成人向视觉小说）的翻译实战中提炼。42 个脚本文件的完整翻译过程，包括用户反馈纠正 AI 翻译问题的全部案例。

---

## License

MIT
