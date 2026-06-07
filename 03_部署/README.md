# 部署与推理加速（工程落地）

本目录包含大语言模型部署和推理加速相关的学习资料和代码实现。

## 学习内容

### 量化技术
- INT8 / INT4 量化
- AWQ 量化
- GPTQ 量化
- GGUF 格式

### 推理引擎
- vLLM（PagedAttention）
- Ollama
- TensorRT-LLM
- TGI（Text Generation Inference）

### 服务化
- OpenAI 兼容 API
- Docker 部署
- Kubernetes 编排
- 负载均衡与弹性伸缩

## 文件结构

```
├── quantization/      # 量化技术实现
├── vllm/              # vLLM 部署示例
├── ollama/            # Ollama 使用示例
└── serving/           # 服务化部署脚本
```
