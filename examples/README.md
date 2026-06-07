# 实战案例

本目录包含大语言模型的完整实战案例，帮助您将理论知识应用到实际场景中。

## 案例列表

### RAG 案例
- `rag_document_search/` - 文档检索问答系统
- `rag_pdf_reader/` - PDF 文档问答

### Agent 案例
- `ecommerce_agent/` - 电商选品智能体
- `code_assistant/` - 代码辅助智能体
- `research_agent/` - 科研文献助手

### 微调案例
- `finetune_sentiment/` - 情感分析微调
- `finetune_summarization/` - 文本摘要微调

### 部署案例
- `deploy_vllm/` - vLLM 部署示例
- `deploy_ollama/` - Ollama 部署示例

## 使用方法

每个案例目录都包含独立的 README 文件，说明具体的使用步骤和依赖安装。

```bash
# 进入具体案例目录
cd ecommerce_agent

# 安装依赖
pip install -r requirements.txt

# 运行案例
python main.py
```
