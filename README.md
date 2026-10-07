# RAG + LLM Interactive Playground

A hands-on, zero-dependency lab that breaks Retrieval-Augmented Generation (RAG) and Large Language Models (LLMs) into every moving part. Tweak the knobs, watch the math, and build intuition. Everything runs locally in your browser — no API keys, no server, no build step.

## Live demo

Once GitHub Pages is enabled (see below), the site is served at:

```
https://aadit001.github.io/rag-llm-playground/
```

## What's inside

Six interactive tabs:

1. **Overview** — the full data flow for a plain LLM and for RAG, side by side.
2. **Tokenizer** — switch between word / sub-word / character tokenization and watch text become token IDs.
3. **Embeddings** — pick an embedding dimension, enter two sentences, and see the vectors plus their cosine similarity.
4. **LLM Sampling** — play with `temperature`, `top-k`, and `top-p`; watch logits → softmax → sampling live.
5. **RAG Pipeline** — paste a knowledge base, tune `chunk_size`, `overlap`, `k`, and `similarity threshold`, and see the exact prompt the model receives.
6. **Glossary** — every term and variable in plain English, with pointers to real tools.

## How it works

The tokenizer, embeddings (deterministic seeded bag-of-words vectors), cosine similarity, softmax, and sampling are all real math running in JavaScript, so results are consistent and inspectable. The final generation step in the RAG tab is a template synthesizer rather than a trained model — the goal is to make visible exactly what a model is *given*.

## Run locally

Just open `index.html` in any modern browser. No install required.

## License

MIT
