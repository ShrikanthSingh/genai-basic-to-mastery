# 🧠 Generative AI & LLM Curriculum — DeepLearning.AI Learning Path

---

## 📌 About This Curriculum

This curriculum is a structured, priority-ranked learning path built from the [DeepLearning.AI](https://www.deeplearning.ai/courses/) course catalog. It is designed for **experienced data scientists and ML practitioners with a solid Python foundation and prior NLP knowledge** who want to systematically master the Generative AI and LLM domain — from core architecture through to production deployment.

The curriculum covers **110+ courses** evaluated and filtered down to the most impactful ones, organized across **5 progressive phases**:

| Phase | Focus | Goal |
|-------|-------|------|
| 1 | LLM Architecture Foundations | Understand how transformers and LLMs work under the hood |
| 2 | Interacting & Adapting LLMs | Prompt, fine-tune, align, and compress models |
| 3 | Building LLM Applications | Build RAG pipelines, chatbots, and semantic search systems |
| 4 | Agentic AI & Advanced Applications | Build autonomous, multi-agent, and multimodal systems |
| 5 | Production, Ops & Safety | Deploy, monitor, evaluate, and govern LLM systems reliably |

---

## 🧭 How to Use This Curriculum for Maximum Benefit

### 1. Follow the Phase Order
Each phase builds on the previous one. Skipping Phase 1–2 without understanding transformers or fine-tuning will create knowledge gaps when debugging agent behavior or evaluating RAG pipelines in later phases.

### 2. Prioritize `🔴 High` Courses First
Within each phase, start with High-priority courses. `🟡 Medium` courses add depth but are not blockers. Complete at least all High-priority courses in a phase before moving to the next.

### 3. Build as You Learn
For every phase, implement a mini-project:
- **Phase 1** → Visualize attention weights on a sample input
- **Phase 2** → Fine-tune an open-source model on a domain-specific dataset
- **Phase 3** → Build a RAG chatbot over your own documents
- **Phase 4** → Build a multi-agent research assistant
- **Phase 5** → Add evaluation + guardrails to your Phase 3/4 project

### 4. Track Your Progress
Use the `Status` column in each table. Update it as:
- `⬜ Not Started`
- `🔄 In Progress`
- `✅ Completed`

### 5. Estimate Your Timeline
Assuming ~8–10 hours/week of focused study:
- Phase 1: ~2 weeks
- Phase 2: ~3 weeks
- Phase 3: ~3 weeks
- Phase 4: ~4 weeks
- Phase 5: ~2 weeks
- **Total: ~14–16 weeks to full proficiency**

> 💡 **Tip:** Given your data science background, Phase 1 can be completed faster (~1 week). Your strongest leverage is in Phase 3–4, where your Python and ML pipeline experience directly transfers.

---

## 🔴 Priority Legend

| Symbol | Meaning |
|--------|---------|
| 🔴 High | Core — complete before advancing |
| 🟡 Medium | Valuable depth — complete within the phase if time allows |
| ⏭️ Skip | Below your level or outside GenAI/LLM scope |

---

## Phase 1 — LLM Architecture Foundations

> Bridge your classical NLP knowledge to the modern transformer-based LLM paradigm. Understanding the internals here will make every downstream course more intuitive.

| Status | Course | Provider | Priority | Why It's Essential |
|--------|--------|----------|----------|--------------------|
| ⬜ | How Transformer LLMs Work | Jay Alammar & Maarten Grootendorst | 🔴 High | Best conceptual primer on transformer architecture — the backbone of every LLM you will use |
| ⬜ | Attention in Transformers: Concepts and Code in PyTorch | StatQuest | 🔴 High | Implements attention from scratch in code; unlocks deep understanding of how LLMs process tokens |
| ⬜ | Generative AI with Large Language Models | AWS | 🔴 High | Covers the full GenAI lifecycle — pretraining, fine-tuning, RLHF, inference — at the right technical depth |
| ⬜ | Understanding and Applying Text Embeddings | Google Cloud | 🔴 High | Bridges your NLP knowledge to modern semantic embeddings used across RAG, search, and retrieval |
| ⬜ | Embedding Models: from Architecture to Implementation | Vectara | 🟡 Medium | Goes deeper into building embedding models; useful if you plan to customize retrieval systems |
| ⬜ | Build and Train an LLM with JAX | Google | 🟡 Medium | Builds a 20M-param LLM from scratch using JAX; great for intuition but not a prerequisite for applications |

---

## Phase 2 — Interacting & Adapting LLMs

> Learn to control, fine-tune, align, and compress LLMs. This phase turns you from an LLM user into an LLM adapter.

| Status | Course | Provider | Priority | Why It's Essential |
|--------|--------|----------|----------|--------------------|
| ⬜ | ChatGPT Prompt Engineering for Developers | OpenAI | 🔴 High | The canonical first hands-on course — covers summarization, inference, transformation, and chaining |
| ⬜ | Finetuning Large Language Models | AMD / Lamini | 🔴 High | Covers when to fine-tune vs. prompt, data prep, training loop, and domain-specific evaluation |
| ⬜ | Fine-tuning & RL for LLMs: Intro to Post-training | AMD | 🔴 High | Extends fine-tuning into SFT, DPO, and RL territory; directly unlocks the next two courses |
| ⬜ | Reinforcement Learning From Human Feedback | Google Cloud | 🔴 High | RLHF is how modern LLMs are aligned — essential for understanding fine-tuning outcomes |
| ⬜ | Quantization Fundamentals with Hugging Face | Hugging Face | 🔴 High | Directly enables running and serving open-source LLMs efficiently on real hardware |
| ⬜ | Open Source Models with Hugging Face | Hugging Face | 🔴 High | Unlocks the entire Hugging Face ecosystem — a dependency for most subsequent hands-on courses |
| ⬜ | Post-training of LLMs | UW / NexusFlow | 🟡 Medium | Covers SFT, DPO, and online RL in depth; good follow-up after the AMD course with some overlap |
| ⬜ | Reinforcement Fine-Tuning LLMs with GRPO | Predibase | 🟡 Medium | Practical GRPO implementation for improving reasoning; relevant after mastering RLHF basics |
| ⬜ | Quantization in Depth | Hugging Face | 🟡 Medium | Advanced quantization variants (symmetric/asymmetric, granularity); take after Quantization Fundamentals |
| ⬜ | Pretraining LLMs | Upstage | 🟡 Medium | Useful for understanding the full model lifecycle but not a prerequisite for application development |
| ⬜ | Prompt Engineering with Llama 2 & 3 | Meta | 🟡 Medium | Valuable for open-source model specifics; partial overlap with ChatGPT Prompt Engineering course |

---

## Phase 3 — Building LLM Applications

> The core production stack. You will build complete RAG systems, chatbots, and semantic search pipelines — the #1 set of skills demanded in GenAI engineering roles today.

| Status | Course | Provider | Priority | Why It's Essential |
|--------|--------|----------|----------|--------------------|
| ⬜ | LangChain for LLM Application Development | LangChain | 🔴 High | Entry point for the most widely used LLM orchestration framework — chains, memory, agents, parsers |
| ⬜ | Retrieval Augmented Generation (RAG) | DeepLearning.AI | 🔴 High | Covers RAG end-to-end from architecture to deployment and evaluation — the number one production pattern |
| ⬜ | Preprocessing Unstructured Data for LLM Applications | Unstructured | 🔴 High | Directly feeds the RAG pipeline — PDF, PowerPoint, HTML extraction; a real blocker in production |
| ⬜ | Vector Databases: from Embeddings to Applications | Weaviate | 🔴 High | Covers hybrid search, multilingual search, and real-world application design with vector DBs |
| ⬜ | LangChain Chat with Your Data | LangChain | 🔴 High | Builds a full document chatbot with LangChain; practical RAG pipeline built from scratch |
| ⬜ | Building Systems with the ChatGPT API | OpenAI | 🔴 High | Teaches chaining, evaluation, and safety checks — critical patterns for any production LLM system |
| ⬜ | Large Language Models with Semantic Search | Cohere | 🔴 High | Rerank, dense retrieval, embeddings for search — directly applicable to RAG improvements |
| ⬜ | Advanced Retrieval for AI with Chroma | Chroma | 🔴 High | Query expansion, cross-encoder reranking, and fixing poor retrieval — must-have for RAG quality |
| ⬜ | Building and Evaluating Advanced RAG | TruEra / LlamaIndex | 🔴 High | Sentence-window and auto-merging retrieval methods; introduces RAGAS-style evaluation |
| ⬜ | Knowledge Graphs for RAG | Neo4j | 🟡 Medium | Adds graph-based retrieval to your RAG stack; powerful for structured or enterprise domain data |
| ⬜ | Prompt Compression and Query Optimization | MongoDB | 🟡 Medium | Optimizes RAG pipeline cost and speed; useful for production but not a beginner dependency |
| ⬜ | Building Applications with Vector Databases | Pinecone | 🟡 Medium | Good hands-on complement to the Weaviate course; some meaningful overlap |

---

## Phase 4 — Agentic AI & Advanced Applications

> Move beyond single-turn applications into autonomous, multi-agent, and multimodal systems. This is the frontier of applied GenAI in 2025–2026.

| Status | Course | Provider | Priority | Why It's Essential |
|--------|--------|----------|----------|--------------------|
| ⬜ | Agentic AI | DeepLearning.AI (Andrew Ng) | 🔴 High | The foundational agentic course — tool use, planning, multi-step workflows taught by Andrew Ng |
| ⬜ | AI Agents in LangGraph | LangChain / Tavily | 🔴 High | LangGraph is the production standard for stateful, controllable agent workflows |
| ⬜ | Functions, Tools and Agents with LangChain | LangChain | 🔴 High | Deep dive into function calling, LCEL, and tool use — prerequisite for advanced agent work |
| ⬜ | Multi AI Agent Systems with crewAI | crewAI | 🔴 High | Best course for multi-agent collaboration — role-based agents, tools, and memory in crewAI |
| ⬜ | AI Agentic Design Patterns with AutoGen | Microsoft / Penn State | 🔴 High | Introduces the key agentic design patterns: reflection, tool use, planning, and multi-agent |
| ⬜ | Building Agentic RAG with LlamaIndex | LlamaIndex | 🔴 High | Combines agents and RAG into intelligent document Q&A systems with routing and summarization |
| ⬜ | Agent Memory: Building Memory-Aware Agents | Oracle | 🔴 High | Persistent memory across sessions — transforms stateless agents into systems that learn over time |
| ⬜ | MCP: Build Rich-Context AI Apps with Anthropic | Anthropic | 🔴 High | Model Context Protocol is becoming the standard for tool and data access in agents |
| ⬜ | Nvidia's NeMo Agent Toolkit: Making Agents Reliable | Nvidia | 🔴 High | Production readiness for agents — observability, evaluation, and deployment tools |
| ⬜ | A2A: The Agent2Agent Protocol | Google Cloud / IBM | 🟡 Medium | Cross-framework agent communication standard; increasingly relevant in 2026 |
| ⬜ | Building with Llama 4 | Meta | 🟡 Medium | Multimodal and long-context applications with open-source Llama 4 models |
| ⬜ | Long-Term Agentic Memory With LangGraph | LangChain | 🟡 Medium | Extends LangGraph with LangMem; some overlap with the Oracle memory course |
| ⬜ | Design, Develop, and Deploy Multi-Agent Systems with crewAI | crewAI | 🟡 Medium | Production deployment focus for crewAI — good follow-up to Multi AI Agent Systems |
| ⬜ | DSPy: Build and Optimize Agentic Apps | Databricks | 🟡 Medium | Programmatic prompt optimization with DSPy; useful for systematic agent improvement |
| ⬜ | Reasoning with o1 | OpenAI | 🟡 Medium | Prompting strategies for reasoning models; relevant as o-series models become the production standard |
| ⬜ | Generative AI for Software Development | DeepLearning.AI | 🟡 Medium | Practical LLM pair programming and code quality; useful for daily data science workflows |
| ⬜ | Introducing Multimodal Llama 3.2 | Meta | 🟡 Medium | Hands-on intro to vision-language models; foundational for multimodal RAG pipelines |
| ⬜ | Building Coding Agents with Tool Execution | E2B | 🟡 Medium | Sandboxed code execution for agents — an important safety pattern for coding agents |
| ⬜ | Event-Driven Agentic Document Workflows | LlamaIndex | 🟡 Medium | Event-driven RAG with human-in-the-loop feedback; practical for enterprise document workflows |

---

## Phase 5 — Production, Ops & Safety

> Transform prototypes into reliable, safe, and scalable production systems. This phase is your bridge from experimentation to engineering.

| Status | Course | Provider | Priority | Why It's Essential |
|--------|--------|----------|----------|--------------------|
| ⬜ | Evaluating and Debugging Generative AI | Weights & Biases | 🔴 High | Covers model versioning, experiment tracking, and debugging GenAI outputs with W&B |
| ⬜ | Evaluating AI Agents | Arize AI | 🔴 High | Systematic agent evaluation framework addressing the non-determinism problem in agent assessment |
| ⬜ | LLMOps | Google Cloud | 🔴 High | LLMOps best practices — fine-tuning pipelines, deployment, and lifecycle automation |
| ⬜ | Automated Testing for LLMOps | CircleCI | 🔴 High | CI/CD pipelines for LLM apps — automated evaluation on every code change |
| ⬜ | Efficiently Serving LLMs | Predibase | 🔴 High | KV caching, batching, and inference optimization — critical for production deployment at scale |
| ⬜ | Improving Accuracy of LLM Applications | AMD / Lamini / Meta | 🔴 High | Systematic accuracy improvement loop: evaluation → prompting → memory tuning |
| ⬜ | Safe and Reliable AI via Guardrails | GuardrailsAI | 🔴 High | Production guardrails for LLM outputs — moves applications from POC to safe production |
| ⬜ | Red Teaming LLM Applications | Giskard | 🔴 High | Identifies vulnerabilities proactively — essential before any public-facing deployment |
| ⬜ | Pydantic for LLM Workflows | DeepLearning.AI | 🔴 High | Structured output validation is foundational for reliable LLM pipelines and agentic systems |
| ⬜ | Governing AI Agents | Databricks | 🟡 Medium | Data governance for agents — important for enterprise settings handling sensitive or regulated data |
| ⬜ | Getting Structured LLM Output | DotTxt | 🟡 Medium | Overlaps with Pydantic course; useful as a second perspective on output structuring |

---

## ⏭️ Optional / Skip

> These courses are either below the target learner's level, domain-specific, or outside the GenAI/LLM scope of this curriculum.

| Course | Reason to Skip |
|--------|----------------|
| Generative AI for Everyone | Too introductory for a 5-year data science background |
| Natural Language Processing Specialization | Assumes no prior NLP knowledge — skip unless refreshing classical NLP concepts |
| Deep Learning Specialization | Covers CNNs/RNNs you likely already know; not LLM-specific |
| PyTorch for Deep Learning / TensorFlow Certificate | Framework basics already covered in a data science background |
| AI Python for Beginners / Build with Andrew | Far below target learner skill level |
| AI for Medicine / AI for Good | Domain-specific, not GenAI or LLM foundational |
| Vibe Coding 101 with Replit | Beginner no-code tooling — not relevant for practitioners |
| Federated Fine-tuning / Intro to Federated Learning | Niche privacy use case; not core to GenAI skill development |
| Carbon Aware Computing for GenAI Developers | Sustainability-focused infrastructure topic — not an LLM skill |
| Jupyter AI: AI Coding in Notebooks | Minor productivity tool, not a learning priority |
| Building AI Voice Agents / Live Voice Agents with Google ADK | Specialized output modality; revisit after mastering the core text-based LLM stack |
| Building AI Browser Agents | Niche agent type; revisit after mastering core agentic patterns with LangGraph and crewAI |
| Semantic Caching for AI Agents | Optimization detail — revisit in production phase after core stack is built |
| Multi-vector Image Retrieval (Qdrant) | Specialized multimodal retrieval — optional unless building vision-heavy applications |
| Fast Prototyping of GenAI Apps with Streamlit | Useful demo skill, but not an LLM learning priority in this curriculum |
| Build Long-Context AI Apps with Jamba | Very model-specific; long-context is now standard in most frontier models |
| Serverless LLM Apps with Amazon Bedrock | AWS-specific deployment path; revisit if your organization uses Amazon Bedrock |

---

## 📈 Progress Tracker

| Phase | Total Courses | High Priority | Completed | Completion % |
|-------|--------------|---------------|-----------|--------------|
| Phase 1 — Foundations | 6 | 4 | 0 | 0% |
| Phase 2 — Adapting LLMs | 11 | 6 | 0 | 0% |
| Phase 3 — LLM Applications | 12 | 9 | 0 | 0% |
| Phase 4 — Agentic AI | 19 | 9 | 0 | 0% |
| Phase 5 — Production & Safety | 11 | 9 | 0 | 0% |
| **Total** | **59** | **37** | **0** | **0%** |

---

*Curriculum built from the DeepLearning.AI course catalog. Last reviewed: March 2026.*
