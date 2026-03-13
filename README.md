# 🚀 数字人马斯克项目

## 项目状态

### ✅ 已完成
- [x] 项目框架搭建 (D:\elon_musk_ai)
- [x] 基础数据收集 (传记、维基百科)
- [x] RAG 检索系统 (简单版)
- [x] 对话系统框架

### 🔄 进行中
- [ ] 收集更多高质量语料
- [ ] 语音/视频数据采集
- [ ] 接入 LLM API (GPT-4o)
- [ ] 声音克隆

### 📋 待完成
- [ ] 向量数据库升级 (Chroma + OpenAI Embeddings)
- [ ] 实时语音对话 (Whisper + TTS)
- [ ] 微信/飞书集成

---

## 目录结构

```
D:\elon_musk_ai\
├── data\
│   ├── raw\
│   │   ├── text\         # 原始文本
│   │   ├── audio\        # 原始音频
│   │   └── video\        # 原始视频
│   └── processed\        # 处理后的数据
│       └── simple_index.pkl  # 索引
├── src\
│   ├── crawler\
│   │   ├── collector.py  # 文本收集
│   │   └── downloader.py # 视频下载
│   ├── rag\
│   │   └── musk_rag.py   # RAG系统
│   └── muskg_chat.py     # 对话系统
└── README.md
```

---

## 下一步：数据收集

### 1️⃣ 优先收集（高价值）

| 数据类型 | 来源 | 预计量 |
|----------|------|--------|
| Lex Fridman 播客 | YouTube | 3小时 |
| Joe Rogan 访谈 | YouTube | 2小时 |
| TED 演讲 | YouTube | 1小时 |
| All-in Podcast | YouTube | 10小时 |
| Twitter/X 推文 | Nitter | 5万条 |

### 2️⃣ 需要你帮忙

1. **下载 YouTube 视频** - 我写好脚本，但需要你确认链接
2. **ElevenLabs 账号** - 需要申请账号来克隆声音
3. **OpenAI API Key** - 用于 GPT-4o 和 Whisper

---

## 对话测试

已可以测试简单的对话：

```bash
python D:\elon_musk_ai\src\musk_chat.py
```

---

## 需要决策

1. **语音方案**: 用 ElevenLabs (更好但需训练数据) 还是微软TTS (快但效果一般)?
2. **对话入口**: 微信? 飞书? 还是网页?
3. **是继续收集更多数据，还是先搭建完整Demo?**
