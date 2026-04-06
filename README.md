# Cascaded RAG Evaluation Platform

**Production-grade local Retrieval-Augmented Generation system built on NVIDIA DGX Spark (Grace Blackwell)**

End-to-end evaluation platform featuring a **self-correcting, multi-stage (cascaded) RAG pipeline** with LangGraph orchestration, local LLM inference, and privacy-first web augmentation.

### Key Features
- Multi-stage (cascaded) retrieval: coarse semantic search → re-ranking → context/metadata filtering
- Self-correcting LangGraph workflow (document grading, hallucination detection, usefulness checks, and intelligent query rewriting)
- Local LLM inference via Ollama with multiple models loaded simultaneously
- Privacy-first web search augmentation using SearxNG
- Full evaluation dashboard and automated benchmarking
- Optimized for the DGX Spark’s 128 GB unified memory architecture

### Benchmark Highlights (v2)
Tested on 10 complex multi-step queries:

| Metric                  | Single Model | Cascade Mode | Improvement |
|-------------------------|--------------|--------------|-------------|
| **Faithfulness (mean)** | 0.16         | **0.70**     | **+0.54**   |
| Faithfulness ≥ 0.70     | 2/10         | **8/10**     | **+6**      |
| Relevancy (mean)        | 0.19         | **0.90**     | +0.71       |
| Context Precision (mean)| 0.31         | **0.47**     | +0.16       |
| Questions with Web Context | 4/10      | **10/10**    | **+6**      |
| Average Latency         | 189s         | **188s**     | –1s         |

**Key takeaway**: Cascade mode eliminated all zero-faithfulness answers and delivered significantly better context relevance through intelligent retrieval and self-correction.

**Full benchmark report**: [BENCHMARK_RESULTS.md](https://github.com/alon-simantov/cascaded-rag-showcase/blob/main/BENCHMARK_RESULTS.md)

### Why This Project Matters
Demonstrates practical, production-ready AI engineering skills:
- Designing scalable, low-latency RAG architectures for complex enterprise workloads
- Building self-correcting Agentic AI pipelines
- Optimizing inference and retrieval on high-performance hardware
- Balancing accuracy, privacy, and performance in hybrid environments

### Tech Stack
Ollama • SearxNG • LangGraph • ChromaDB • FastAPI • NVIDIA DGX Spark (Grace Blackwell) • Python 3.12

---

⭐ The complete codebase is kept private to protect an ongoing customer POC.  
Hiring managers and recruiters are welcome to request temporary collaborator access or a live demo.

Built as hands-on proof of forward-deployed AI implementation and solution architecture capabilities.
