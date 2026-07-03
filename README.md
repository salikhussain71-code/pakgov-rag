# PAKGOV-RAG

A bilingual Urdu-English Retrieval-Augmented Generation system for Pakistani government documents — FBR, HEC, NADRA, SECP, and Supreme Court records.

## Why this project exists

Pakistani citizens deal with government documents every day, but almost none of the tools built to search or explain them work well in Urdu. Most retrieval and generation systems are trained and tested on English, so Urdu users are left out. This project is an attempt to close that gap for one specific, useful case: government and legal text.

## What it does

Given a question in Urdu or English, the system retrieves the most relevant passages from a collection of government documents and generates a grounded answer, citing where the information came from.

## Status

Early stage — data collection and pipeline design in progress.

## Roadmap

- **Phase 1:** Scrape and OCR government documents, clean and normalize Urdu/Arabic script text
- **Phase 2:** Build hybrid retrieval — BM25 combined with dense embeddings (XLM-R), stored in FAISS
- **Phase 3:** Connect a generation model (mT5 or QLoRA-tuned Llama-3), serve through FastAPI, demo on Gradio
- **Phase 4:** Evaluate with RAGAS (faithfulness, context precision, context recall, answer relevance), run a human evaluation study, write up results

## Tech stack

Python, LangChain, FAISS, Tesseract OCR, PyTorch, HuggingFace Transformers, FastAPI, Docker, RAGAS

## Author

Salik Hussain — BS Computer Science, Air University Islamabad
GitHub: github.com/salikhussain71-code

## License

MIT
```

---
