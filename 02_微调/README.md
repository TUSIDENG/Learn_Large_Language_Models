# 微调（垂直领域定制）

本目录包含大语言模型微调相关的学习资料和代码实现。

## 学习内容

### 高效参数微调（PEFT）
- LoRA（Low-Rank Adaptation）
- QLoRA（量化 LoRA）
- Adapter 等其他 PEFT 方法

### 对齐技术（Alignment）
- SFT（监督微调）
- RLHF（人类反馈强化学习）
- RLAIF（AI 反馈强化学习）
- DPO、PPO 算法

### 工具链
- LLaMA-Factory
- Axolotl
- Hugging Face TRL
- PEFT 库

## 文件结构

```
├── lora/              # LoRA 微调实现
├── sft/               # 监督微调脚本
├── rlhf/              # 强化学习对齐
└── configs/           # 微调配置文件
```
