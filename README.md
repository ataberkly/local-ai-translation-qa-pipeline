# Local & Offline AI Translation & QA Pipeline

A 100% private, self-hosted, and offline translation and quality control (QA) workflow built using Docker, n8n, Ollama, and Qwen2.5 (7B). 

Designed for enterprise localization environments requiring strict data privacy, zero API costs, and structured LLM outputs.

## 🌟 Key Features
- **Data Privacy & GDPR Compliance:** Runs completely offline via local Docker containers. Zero data leakage to public LLM providers (e.g., OpenAI/Anthropic).
- **Optimized Local LLM (Qwen2.5:7b):** Leverages Qwen2.5 for superior Turkish linguistic nuance, syntax accuracy, and cultural adaptation.
- **Precision Parameter Tuning:** Model inference parameters adjusted (`temperature=0.2`, `top_p=0.1`) to strictly prevent hallucinations and ensure deterministic QA evaluation.
- **Custom User Interface:** Utilizes n8n Form Trigger & Completion Page architecture for seamless source text submission and instant formatted QA report delivery.

## 🛠️ Tech Stack
- **Automation Engine:** n8n (Self-Hosted / Docker)
- **Local LLM Runtime:** Ollama
- **Model:** Qwen2.5 (7B)
- **Interface:** n8n Form & Dynamic Completion Page

## 🚀 How It Works
1. **Source Input:** Users input English source text via the n8n Form interface.
2. **Local Inference:** The payload is processed offline by Ollama running Qwen2.5 (7B).
3. **Structured Output:** The model returns a fluent Turkish translation along with structured QA notes (terminology analysis, tone, and stylistic evaluation).
4. **Instant UI Rendering:** Results are displayed dynamically on the custom Completion Page.

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
