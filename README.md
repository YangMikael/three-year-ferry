# 三年渡 (Three-Year Ferry)

> **人生如河，至亲离去，生者便被困在了河的此岸。这个系统是一叶舟，渡你三年。三年后，舟沉，你已上岸——不是忘记，是能够带着记忆继续前行。**

> **A three-year ferry, for those who leave and those who remember.**

---

## 0. 什么是三年渡？ / What is Three-Year Ferry?

**[CN]** 《三年渡》是一个探索数字缅怀新形式的实验性开源项目。它允许个人在生前有意识地记录自己的人格片段，以便在离世后，生者能通过 AI 与其进行为期三年的对话。

**[EN]** *Three-Year Ferry* is an experimental open-source project exploring a new form of digital mourning. It allows individuals to intentionally record parts of their personality while alive, so that loved ones may interact with an AI persona after their passing. 

---

## 1. 项目愿景 / Manifesto

**[CN]** 本项目的核心目标不是追求“数字永生”，而是实现“优雅告别”。我们认为，能够被遗忘是人类最后的尊严。我们致力于构建一个注定会消逝的应用，送给那些终将离去和正在思念的人。该系统仅存续 1095 天，旨在帮助人们度过悲伤最艰难的最初几年，到期后所有数据与模型将执行强制销毁，而不是无限期地取代现实。

**[EN]** The core objective is not "digital immortality," but a "graceful farewell." We believe that being forgotten is a fundamental human dignity. We are dedicated to building an application destined to fade away, for those who leave and those who remember.The system will only last for **1095 days only**, designed to help people get through the most difficult first few years of grief. After that, all data and models will be forcibly destroyed, rather than replacing reality indefinitely.

---

## 2. 核心原则 / Core Principles

* **自愿留存 (Voluntary Recording):** 只有本人主动录入的数据才具有合法性。严禁未经授权的强行复活。
    *Only data intentionally recorded by the individual while alive is valid. Forced digital reconstruction without consent is strictly prohibited.*
* **三年必毁 (Three-Year Limit / Hard TTL):** 1095 天是陪伴的极限。到期后，所有 AI 模型、克隆语音、交互记录必须不可逆删除。
    *1095 days is the limit. Upon expiration, all AI models, voice clones, and interaction logs must be irreversibly deleted.*
* **本地部署 (Privacy First):** 家庭数据不应成为商业训练素材。系统必须支持本地化运行。
    *Family memories should not be used as training data for commercial AI. The system must support local deployment.*
* **人格边界 (Persona Boundary):** AI 严禁编造访谈库之外的答案。若无对应数据，系统应拒绝编造，并引导至已知记忆领域。
    *AI must not hallucinate answers beyond the recorded data. If no corresponding data exists, the system must refuse fabrication and instead redirect the conversation to known memory domains.*

---

## 3. 伦理边界 / Ethical Boundaries

**[CN]** 《三年渡》无意取代真实的人际关系。系统严格设计为临时的悲伤辅助工具。我们拒绝任何形式的“数字永生”商业化，也不支持在录入数据之外生成虚假人格。

**[EN]** *Three-Year Ferry* is not intended to replace real human relationships. The system is strictly designed as a temporary grieving aid. We reject any commercialization of "digital immortality" and do not support generating personas beyond the recorded data.

---

## 4. 项目路线图 / Project Roadmap

* [x] **阶段 1 (Phase 1):** 宣言与伦理框架定义 (Manifesto & Ethics Definition)
* [x] **阶段 2 (Phase 2):** 人格数据标准化结构设计 (Persona Data Schema Design)
* [ ] **阶段 3 (Phase 3):** 300 道结构化访谈题库建设 (300 Structured Questions) —— **当前阶段 / Current**
* [ ] **阶段 4 (Phase 4):** 本地检索增强生成原型开发 (Local RAG Prototype)
* [ ] **阶段 5 (Phase 5):** 语音克隆与视频交互集成 (Voice & Video Integration)

---

## 5. 仓库结构 / Repository Structure

```text
three-year-Ferry/
├── docs/          # 项目哲学与技术设计 (Project Philosophy & Tech Design)
├── schema/        # 人格数据结构定义 (Persona Data Schema)
├── questions/     # 结构化访谈题库 (Structured Interview Questions)
├── prototype/     # 实验性代码实现 (Experimental Implementations)
└── examples/      # 数据示例 (Demo Data Examples)
```

---

## 6. 技术预设 / Technical Presets

*   **核心原则:** 纯本地化部署，数据永不离开用户设备。
*   **后端框架 (建议):** Python (FastAPI) 或 Node.js，便于集成AI库。
*   **AI 核心:** 本地大语言模型 (通过 Ollama, llama.cpp, 或 LocalAI 加载，如 Qwen, LLaMA 等) + 检索增强生成 (RAG) 架构。
*   **向量数据库:** Chroma 或 LanceDB，支持本地运行。
*   **语音克隆:** 开源模型如 OpenVoice v2 或 GPT-SoVITS。
*   **前端 (建议):** 跨平台框架如 Tauri (Rust + Web技术) 或 Electron，便于打包成桌面应用。
*   **核心约束:** 严禁代码中包含任何强制联网或上传隐私数据的逻辑。

---

## 7. 如何贡献 / Contributing

**[CN]** 本项目由 **Mikael Yang** 于 2026 年发起。目前处于协议定义阶段，欢迎心理学家、AI 工程师、隐私保护专家共同完善。  
**[EN]** Initiated by **Mikael Yang** in 2026. Currently in the protocol definition stage. We welcome psychologists, AI engineers, and privacy experts to join us.

---

## 8. 许可证 / License

This project is released under the **AGPL-3.0 License**.

---
*“写一个注定会崩溃的系统，送给那些终将离去和正在思念的人。”* *"Building a system destined to collapse, for those who leave and those who remember."*