# Learn Large Language Models

学习大语言模型（LLM）是一个系统性的工程。本仓库整理了学习大模型所需的核心知识体系，涵盖四个关键维度：**原理、微调、部署、应用开发**。

---

## 📚 学习路线总览

学习大模型建议采取"**两头包抄**"的策略：
1. **先应用，后底层**：从应用开发（LangChain + RAG + API）切入，快速看到效果
2. **补齐微调与部署**：遇到瓶颈时学习 Ollama/vLLM 部署及 LoRA 微调
3. **死磕原理**：有工程经验后再深入 Transformer 论文和数学公式

---

## 核心一：原理（底层基石）

不理解原理，微调和部署就会变成"盲人摸象"。目标是搞清楚大模型是如何"思考"和"记忆"的。

### Transformer 架构
- 自注意力机制（Self-Attention）
- 多头注意力（Multi-Head Attention）
- 位置编码（Positional Encoding）

### 主流模型变体
- LLaMA、DeepSeek、GPT 等模型架构演进
- MoE（混合专家模型）架构

### 预训练（Pre-training）
- 因果语言建模（Causal Language Modeling）
- Next-token prediction 机制

### Tokenizer（分词器）
- BPE（Byte Pair Encoding）算法
- 分词原理与常见问题排查

---

## 核心二：微调（垂直领域定制）

当通用大模型无法满足特定业务场景时，微调是注入"行业专家知识"或"特定输出格式"的手段。

### 高效参数微调（PEFT）
- **LoRA（Low-Rank Adaptation）**
- **QLoRA**（量化后的 LoRA）

### 对齐技术（Alignment）
- **SFT（监督微调）**：用"问题-答案"对规范回答格式
- **RLHF / RLAIF（强化学习）**：DPO、PPO 算法

### 微调工具链
- LLaMA-Factory
- Axolotl
- Hugging Face TRL 库

---

## 核心三：部署与推理加速（工程落地）

模型训练好后，如何让它在高并发、低延迟的线上环境跑起来。

### 量化技术（Quantization）
- INT8 / INT4 量化
- AWQ、GPTQ、GGUF 等量化格式

### 推理加速引擎
- **vLLM**：行业标准，PagedAttention 提升吞吐量
- **Ollama**：适合本地快速部署和测试
- **TensorRT-LLM**：英伟达官方，性能极致

### 服务化（Serving）
- OpenAI 兼容 API 接口封装
- Docker 容器化部署
- 云端弹性伸缩

---

## 补充维度：应用开发（RAG 与 Agent）

很多时候不需要微调模型，而是通过"外挂"来解决问题。

### RAG（检索增强生成）
- Embedding 技术
- 向量数据库（MongoDB、Chroma、Pinecone）
- Rerank、混合检索策略

### Agent（智能体）与 Tool Calling
- 工具调用机制
- 自我反思与任务规划
- 多 Agent 协作

### 开发框架
- LangChain
- LlamaIndex
- AutoGen

---

## 💡 学习建议

| 阶段 | 重点内容 | 预期成果 |
|------|----------|----------|
| 入门 | RAG + API + LangChain | 完成电商选品 Agent 等实际项目 |
| 进阶 | LoRA 微调 + vLLM/Ollama 部署 | 能独立完成模型微调与部署 |
| 深入 | Transformer 原理 + 数学推导 | 理解模型底层机制 |

---

## 📁 项目结构

```
├── 01_原理/           # Transformer、Tokenizer、预训练
├── 02_微调/           # PEFT、LoRA、SFT、RLHF
├── 03_部署/           # vLLM、Ollama、量化
├── 04_应用/           # RAG、Agent、LangChain
└── examples/          # 完整实战案例
```

---
