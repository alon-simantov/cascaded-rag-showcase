# Cascaded RAG Evaluation Platform – ServiceNow Moveworks & Now Assist Aligned

**Production-grade local RAG evaluation platform built on NVIDIA DGX Spark (GB10)**

End-to-end testing of Retrieval-Augmented Generation with **self-correcting LangGraph pipelines**, multi-stage (cascaded) retrieval, and LLM-as-judge scoring — fully offline and privacy-first.

### Key Features
- **Cascaded Retrieval**: coarse semantic search → re-ranking → context/metadata filtering
- Self-correcting LangGraph workflow (grades documents, detects hallucinations, checks usefulness, rewrites queries when needed)
- Local LLM inference via **Ollama** (multiple models resident simultaneously)
- Privacy-first web augmentation with **SearxNG**
- ChromaDB vector store + full evaluation dashboard
- Optimized specifically for the DGX Spark’s 128 GB unified memory

### ServiceNow Moveworks / Now Assist Alignment
This project directly mirrors ServiceNow’s AI Platform patterns:
- Multi-stage RAG retrieval used in **Now Assist AI Search** and **AI Agent Studio**
- Agentic self-correction and reasoning loops (Moveworks Enterprise Search style)
- Hallucination reduction + grounded generation
- Hybrid/local inference best practices for enterprise deployments

### Demo & Results
[→ Add your 30–60 second Loom video or GIF here (anonymized)]

**Sample Metrics** (replace with your real numbers):
- Answer relevance improvement: **+42%** vs single-stage RAG
- Average end-to-end latency: **<180 ms** per query on DGX Spark
- Supports concurrent model loading with zero swap overhead

### Full Implementation
The complete codebase and detailed setup instructions are kept in a **private repository** to protect an ongoing customer POC.  

If you are a ServiceNow recruiter or hiring manager, I’m happy to:
- Invite you as a temporary collaborator, or
- Share a read-only link / live demo under NDA

Just reach out via LinkedIn.

### Tech Stack
Ollama • SearxNG • LangGraph • ChromaDB • NVIDIA DGX Spark (Grace Blackwell) • FastAPI Dashboard • Python 3.12

**Built as hands-on proof of forward-deployed AI Implementation skills.**

⭐ Star this repo if you’re exploring Agentic RAG or ServiceNow AI patterns!
