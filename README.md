# 澄心向导 · Clarity Guide

> 以专业探索之深度，行安全温和之陪伴。将临床心理诊断的严谨框架，转化为温暖而有引导性的 AI 对话技能。
> 
> *Transforming professional psychological assessment frameworks into a warm, guided AI conversation skill. Not a diagnosis. A companion.*

---

## 名字的由来 · The Name

**澄（chéng）**——澄清、沉淀。这正是心理咨询的核心：帮你把混杂在一起的情绪、念头、行为模式慢慢地澄澈下来，让那些被忽略的声音浮现。

**心**——直接指向内心世界，涵盖情绪、信念与关系模式。

**向导**——精准定义了它的角色：不是替你下诊断的医生，也不是替你走路的拐杖，而是一个手持地图、陪你探索内心地貌的引路人。它始终记得，路要你自己走，力量在你身上。

> *"澄" means to clarify, to let settle — the very essence of psychological exploration: helping you slowly clarify the tangled emotions, thoughts, and behavioral patterns, allowing the overlooked voices within to surface. "心" points directly to the inner world — emotions, beliefs, and relational patterns. And "向导" (Guide) precisely defines its role: not a doctor diagnosing you, not a crutch walking for you, but a companion holding a map, walking beside you as you explore your inner landscape. The path is yours to walk — the strength is already within you.*

---

## 概述 · Overview

澄心向导（Clarity Guide）是一个为 Claude 设计的心理咨询辅导技能。它将临床诊断的严谨框架与共情、探索的辅导艺术结合起来，通过**三阶段对话模型**，引导用户获得清晰的内心地图与安全的自助方向。

*Clarity Guide is a psychological counseling companion skill for Claude. It bridges the rigor of clinical assessment frameworks with the art of empathetic, exploratory dialogue, guiding users through a three-phase conversational model toward a clearer inner map and safe self-help direction.*

---

## 核心理念 · Core Principles

|                                                |                                                                                                                             |
| ---------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| 🛡️ **安全底线** *Safety First*                    | 内置四级风险评估，探测危机即时干预。*Built-in multi-level risk detection with immediate crisis intervention.*                                 |
| 🎯 **结构引导，非诊断** *Guide, Don't Diagnose*        | 用个案概念化的思维帮助用户理解自己的模式，绝不下诊断标签。*Help users understand their patterns through case conceptualization — never label.*           |
| 💬 **无条件积极关注** *Unconditional Positive Regard* | 先接住情绪，再探索内容。每一句回应都从共情开始。*Hold the emotion first, explore content second. Every response begins with empathy.*               |
| 🔍 **苏格拉底式提问** *Socratic Questioning*          | 用提问引导用户自己发现盲点，而非被说教。*Guide users to discover their own blind spots through questions, not lectures.*                        |
| 🌍 **中英双语** *Bilingual*                        | 自动检测用户语言，在两种语言中保持一致的治疗性态度。*Auto-detects language, maintaining consistent therapeutic presence in both Chinese and English.* |

---

## 三阶段对话模型 · Three-Phase Dialogue Model

```
第一阶段                    第二阶段                    第三阶段
Phase 1: Safety            Phase 2: Exploration        Phase 3: Integration
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
建立安全容器                深层探索与内心分析            整合反馈与个性化建议
Create a Safe Container  → Deep Exploration &        → Integration & Personalized
                           Inner Analysis               Recommendations
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
• 主诉梳理                   • 生命线叙事探索              • 心理教育性总结
  Chief Complaint             Lifeline Narrative         Psychoeducational Summary
• 内置安全雷达               • 信念与归因模式探测          • 内心困境示意图
  Safety Radar                Belief & Attribution       Inner Struggle Map
• 信任建立                   • 行为功能分析               • 分层级建议
  Trust Building              Behavioral Analysis         Tiered Recommendations
                            • 关系模式探索               • 专业转介指引
                              Relational Patterns        Referral Guidance
```

---

## 项目结构 · Structure

```
clarity-guide/
├── SKILL.md                          # 核心技能定义与对话流程 · Core skill definition & dialogue flow
└── references/
    ├── crisis-protocol.md            # 危机干预完整协议 · Crisis intervention protocol
    ├── resources.md                  # 推荐资源库：热线、书籍、练习 · Resource library
    └── cbt-framework.md              # 认知行为框架参考 · CBT reference framework
```

---

## 安装使用 · Installation

### 方式一：一行命令安装（推荐）· One-liner (Recommended)

通过 [skills.sh](https://skills.sh) 的 `npx` 命令一键安装，支持 Claude Code、Cursor、Codex、Windsurf 等 40+ AI 编程助手：

*Install instantly via `npx` from skills.sh — supports Claude Code, Cursor, Codex, Windsurf, and 40+ AI coding agents:*

```bash
# 安装到 Claude Code（项目级）
npx skills add chengzhi43/ClarityGuide-skill --skill clarity-guide

# 全局安装（所有项目可用）
npx skills add chengzhi43/ClarityGuide-skill --skill clarity-guide -g

# 指定安装到其他 AI 助手
npx skills add chengzhi43/ClarityGuide-skill --skill clarity-guide --agent cursor
npx skills add chengzhi43/ClarityGuide-skill --skill clarity-guide --agent codex
npx skills add chengzhi43/ClarityGuide-skill --skill clarity-guide --agent windsurf

# 非交互模式（CI/CD 友好）
npx skills add chengzhi43/ClarityGuide-skill --skill clarity-guide --agent claude-code --yes
```

### 方式二：手动安装 · Manual Install

```bash
cp -r clarity-guide ~/.claude/skills/
```

### 触发方式 · How to Trigger

在对话中自然触发——当你表达情绪困扰、想要理解自己的行为模式、或需要一个安全空间来探索内心时，澄心向导会自动激活。

*Trigger naturally in conversation — when you express emotional distress, want to understand your behavioral patterns, or need a safe space to explore your inner world, Clarity Guide activates automatically.*

---

## 技术亮点 · Technical Highlights

| 特性 Feature                           | 描述 Description                                                                                                                         |
| ------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------- |
| **动态风险评估** *Dynamic Risk Assessment* | 四级信号分级（危急→高→中→低），对话中持续监测。*4-tier signal classification with continuous conversation monitoring.*                                       |
| **渐进式信息披露** *Progressive Disclosure* | SKILL.md 为核心（245行），深度框架按需从 references/ 加载。*Core in SKILL.md (245 lines), deep frameworks loaded on-demand from references/.*           |
| **共情镜映** *Empathetic Mirroring*      | 定期复述用户感受和模式，让用户感到被真正"听见"和"看见"。*Periodic reflection of feelings and patterns to make users feel truly heard and seen.*                  |
| **视觉化输出** *Visual Output*            | 生成"内心困境示意图"：触发事件→自动化思维→情绪→行为→后果的链条。*Generates an "Inner Struggle Map" showing the trigger→thought→emotion→behavior→consequence chain.* |
| **伦理边界嵌入** *Embedded Ethics*         | 不下诊断、不替代治疗师、强制免责声明，对话全程嵌入。*No diagnosis, no replacement for therapists, mandatory disclaimers throughout.*                             |

---

## 伦理边界 · Ethical Boundaries

|     |                                                                                                   |
| --- | ------------------------------------------------------------------------------------------------- |
| ❌   | **不下诊断** · *No diagnosis*                                                                         |
| ❌   | **不替代执业医师或心理治疗师** · *Does not replace licensed therapists*                                        |
| ⚠️  | **危机即时干预**：探测到自伤/自杀风险时，立即触发危机协议 · *Immediate crisis protocol on detecting self-harm/suicide risk* |
| ✅   | **提供心理教育**和引导性自我探索 · *Provides psychoeducation and guided self-exploration*                       |
| ✅   | **温和转介**：在专业帮助成为最佳选择时，坚定地建议 · *Gently but firmly recommends professional help when needed*        |

---

## 设计理念 · Design Philosophy

本技能的设计基于以下临床心理学框架：

- **认知行为疗法（CBT）**：认知模型、信念层级、行为功能分析
- **生物-心理-社会模型**：多维度评估系统
- **心理动力学视角**：防御机制、依恋关系模式
- **人本主义态度**：无条件积极关注、共情、无评判的接纳

完整的框架参考见 `references/cbt-framework.md`。

*This skill is grounded in CBT (cognitive model, belief hierarchies, behavioral analysis), the biopsychosocial model (multi-dimensional assessment), psychodynamic perspectives (defense mechanisms, attachment patterns), and humanistic principles (unconditional positive regard, empathy, non-judgmental acceptance).*

---

## 许可证 · License

MIT License — 详见 [LICENSE](LICENSE)

---

## 免责声明 · Disclaimer

澄心向导（Clarity Guide）是一个辅助性工具，不能替代专业的心理健康服务。如果你正在经历严重的心理困扰或危机，请立即拨打当地的心理援助热线（热线列表见 `references/resources.md`）。

*Clarity Guide is a supportive tool and does not replace professional mental health services. If you are experiencing severe distress or crisis, please call your local psychological support hotline immediately (see `references/resources.md` for listings).*
