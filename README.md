# 可视化RAG系统 (Visual RAG Studio)

> 透明、可交互的检索增强生成(RAG)系统，让您看见并优化每个环节。

![版本](https://img.shields.io/badge/version-0.1.0--alpha-blue)
![许可](https://img.shields.io/badge/license-MIT-green)

## 📖 项目简介

Visual RAG Studio 是一个创新的可视化界面系统，旨在解决当前RAG框架普遍存在的"黑盒"问题。通过直观的拖拽界面和实时反馈，它使您能够：

- **可视化整个RAG流程**，从文档接入到最终生成的每个步骤
- **动态调整和优化**各环节的参数和配置
- **实时查看中间结果**和性能指标
- **对比不同配置**的效果和输出质量

无论您是NLP工程师、知识库开发者，还是对LLM应用感兴趣的技术人员，这个工具都能帮助您更深入理解和优化RAG系统。

## ✨ 核心功能

### 🔄 完整RAG流程可视化

- 文档接入与处理
- 文本分块与处理
- 嵌入生成与向量存储
- 查询处理与增强
- 相关内容检索与重排序
- 上下文组装与增强
- LLM生成与输出格式化
- 结果评估与性能分析

### 🛠️ 直观的参数优化

- 拖拽式界面，视觉化流程设计
- 实时参数调整和配置
- 配置预设和模板共享
- 参数变更实时反馈

### 📊 全面的性能分析

- 检索准确度指标
- 响应时间监控
- 资源使用统计
- 质量评估对比

### 💾 多种接入选项

- 本地文件处理
- 网页和URL抓取
- 数据库连接
- API集成

## 🧰 技术栈

### 前端
- **框架**: Next.js + TypeScript
- **UI**: Tailwind CSS + shadcn/ui
- **流程可视化**: ReactFlow
- **数据可视化**: react-chartjs-2
- **状态管理**: Zustand

### 后端
- **API框架**: FastAPI
- **RAG引擎**: LlamaIndex + Langchain
- **向量存储**: FAISS/Chroma (本地), Pinecone/Weaviate (云端)
- **嵌入模型**: Sentence-Transformers, OpenAI Embeddings API
- **数据存储**: SQLAlchemy + PostgreSQL

### DevOps
- **容器化**: Docker + Docker Compose
- **CI/CD**: GitHub Actions
- **测试**: Jest, pytest

## 🚀 开始使用

### 🔧 安装与设置

```bash
# 克隆仓库
git clone https://github.com/yourusername/visual-rag-studio.git
cd visual-rag-studio

# 使用Docker Compose启动所有服务
docker-compose up -d

# 或分别启动前后端（开发模式）
# 前端
cd frontend
npm install
npm run dev

# 后端
cd backend
pip install -r requirements.txt
uvicorn app.main:app --reload
```

### 💻 基本使用流程

1. **文档导入**: 上传或导入要处理的文档
2. **流程配置**: 拖拽组件创建或使用预设的RAG流程
3. **参数设置**: 配置每个组件的具体参数
4. **测试与优化**: 输入测试查询，观察结果，调整参数
5. **流程导出**: 保存优化后的配置供生产环境使用

## 📝 开发路线图

### 第一阶段: 前端流程设计与基础UI (2周)
- [x] 项目结构搭建
- [ ] 基础UI组件开发
- [ ] ReactFlow流程图实现
- [ ] 节点配置界面设计

### 第二阶段: 后端基础架构与核心RAG组件 (2周)
- [ ] FastAPI框架搭建
- [ ] LlamaIndex基础集成
- [ ] 文档处理流程
- [ ] 基础API端点实现

### 第三阶段: 前后端集成与基础RAG流程 (2周)
- [ ] API通信实现
- [ ] 端到端基础流程
- [ ] 用户交互优化
- [ ] 基础监控实现

### 第四阶段: 高级功能与优化 (2-3周)
- [ ] 高级RAG功能实现
- [ ] 性能分析与可视化
- [ ] 系统性能优化
- [ ] 用户体验提升

## 👥 参与贡献

欢迎贡献代码、报告问题或提出改进建议！请查看[贡献指南](CONTRIBUTING.md)了解详情。

## 📄 许可证

[MIT License](LICENSE)

## 🙏 致谢

- 感谢所有开源RAG框架和工具的贡献者
- 特别感谢[LlamaIndex](https://github.com/jerryjliu/llama_index)和[Langchain](https://github.com/hwchase17/langchain)项目
- React Flow和其他开源UI库的开发者

---

*Visual RAG Studio 目前处于积极开发阶段，欢迎您的反馈和建议！*