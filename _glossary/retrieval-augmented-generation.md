---
title: "What Is Retrieval-Augmented Generation (RAG)? | Apex Data Cloud"
defines: "Retrieval-Augmented Generation (RAG)"
breadcrumb_name: "Retrieval-Augmented Generation"
description: "Retrieval-augmented generation (RAG) is a technique that retrieves relevant information from a knowledge base and supplies it to a large language model as context, so answers are grounded in trusted, current data."
keywords: "retrieval augmented generation, RAG definition, what is RAG"
related:
  - { title: "RAG Development", url: "/services/rag-development/" }
  - { title: "RAG Implementation Guide", url: "/resources/guides/rag-implementation-guide/" }
  - { title: "RAG vs. Fine-Tuning", url: "/comparisons/rag-vs-fine-tuning/" }
---

**Retrieval-augmented generation (RAG)** is a technique that retrieves relevant passages from a knowledge base and supplies them to a large language model (LLM) as context, so the model answers from trusted, current information instead of only its training data.

## Why it matters

A general LLM only "knows" its training data up to a cutoff date and nothing private. RAG lets a model answer from *your* documents, policies, and products — and cite sources — which dramatically reduces hallucinations and makes answers traceable. It's the most common pattern for reliable enterprise generative AI.

## How it works (in brief)

Documents are ingested, split into chunks, and converted into vector [embeddings](/glossary/embeddings/) stored in a [vector database](/glossary/vector-database/). At query time, the system retrieves the most relevant chunks and passes them to the LLM to generate a grounded answer.

## Related

See [RAG development](/services/rag-development/), the [RAG Implementation Guide](/resources/guides/rag-implementation-guide/), and when to choose [RAG vs. fine-tuning](/comparisons/rag-vs-fine-tuning/).
