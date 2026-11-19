# 改命记实录 · Agent Skill

Agent skill generated from 《改命记实录》 by 道之光（叙述者「三合」） with [book-to-skill](https://github.com/virgiliojr94/book-to-skill).

这是一个将《改命记实录》（858 个短章）按主题归并、提炼而成的 Agent Skill。它把书中的方法论——阴阳推理、六爻反断、预测与化解、八字面相风水、择吉姓名、道医象数、改命修心、以及识别算命骗局——整理成可按需加载的专题章节，供 Agent 在回答相关问题时引用。

这是一个纯 Markdown 的中文读书助手，无需运行脚本。适合按主题查术语、梳理书中的观点和案例，或了解作者如何辨别算命话术。内容是**提炼后的结构化摘要与索引，不是原书文本**。

## 安装 / Install

安装到任意 Agent Skills 宿主（Claude Code、WorkBuddy 等）：

```bash
npx skills add <此文件夹路径> --skill gaimingji
```

或直接把整个 `gaimingji/` 文件夹复制到宿主的 skills 目录，例如 `~/.workbuddy/skills/`、`~/.claude/skills/`。

## 用法

- 直接问某个主题（如「反断」「光煞」「有病方为贵」「婚配」「算命心理学」），Agent 会读取对应专题章节再回答
- 问 `ch04` 可加载指定专题文件
- 问「有哪些章节」查看完整索引

可以从这几个问题开始：

- 「书里说的『反断』是什么？作者为什么后来不再依赖它？」
- 「对照 ch17 和 ch18，解释作者怎么看个人行动和外在因素。」
- 「书里有哪些辨别算命话术的方法？举一个巴纳姆式表述的例子。」

## 文件清单

| 文件 | 说明 |
|---|---|
| `SKILL.md` | 核心框架速览 + 20 章索引 + 主题索引（入口，含 YAML frontmatter） |
| `chapters/`（20 个） | 按主题归并的专题章节，每章含 Core Idea / Frameworks / Key Concepts / Mental Models / Anti-patterns / Worked Example / Key Takeaways |
| `glossary.md` | 全书关键术语表 |
| `patterns.md` | 方法与技术的「何时用 / 怎么做 / 取舍」清单 |
| `cheatsheet.md` | 决策规则表、内外因权重、常见坑速记 |

### 专题章节

| 文件 | 专题 |
|---|---|
| `ch01-worldview-yin-yang.md` | 专题 1: 阴阳世界观与全书总纲 |
| `ch02-prediction-principle.md` | 专题 2: 预测与化解的原理 |
| `ch03-reversal-wisdom.md` | 专题 3: 反断、悟性与给人希望 |
| `ch04-liuyao.md` | 专题 4: 六爻：装卦、六亲与用神 |
| `ch05-meihua-yishu.md` | 专题 5: 梅花易数与起卦的心法 |
| `ch06-xiaoliuren.md` | 专题 6: 小六壬（掐指神通术） |
| `ch07-bazi.md` | 专题 7: 八字：看性格、运势与格局 |
| `ch08-face-reading.md` | 专题 8: 面相与手相：五官、三停、掌纹 |
| `ch09-zodiac-marriage.md` | 专题 9: 属相、婚配与关系判断 |
| `ch10-fengshui.md` | 专题 10: 风水：煞、能量与居家调整 |
| `ch11-zchoose-date.md` | 专题 11: 择吉、九运与五行穿衣 |
| `ch12-name-studies.md` | 专题 12: 姓名学与符号预测 |
| `ch13-xiangshu-therapy.md` | 专题 13: 八卦象数疗法 |
| `ch14-dao-medicine.md` | 专题 14: 道医、偏方与身心调理 |
| `ch15-cultivation.md` | 专题 15: 修行、功法与能量 |
| `ch16-love-relationships.md` | 专题 16: 婚恋、桃花与感情判断 |
| `ch17-inner-outer.md` | 专题 17: 内求与外求：外力只是助缘 |
| `ch18-four-methods.md` | 专题 18: 改命的四种方法与心性修炼 |
| `ch19-psychology-critical.md` | 专题 19: 心理学的挪用与算命心理学批判 |
| `ch20-pragmatic-stance.md` | 专题 20: 防骗、实用立场与作者的中道 |

## 版权说明

本包由第三方版权书籍提炼生成，章节为综合摘要而非原文复制。仅限个人学习与研究使用，请勿公开再分发原书内容或本派生包。涉及健康、法律、重大决策请以专业意见为准；书中术法属传统文化范畴，请理性看待。
