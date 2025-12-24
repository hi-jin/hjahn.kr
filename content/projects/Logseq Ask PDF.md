---
{"publish":true,"created":"2025-12-24T16:30:50.526+09:00","modified":"2024-09-15","cssclasses":""}
---

A Logseq plugin that allows you to ask questions about PDF highlights (text or images) using Large Language Models (LLMs).

![demo](https://github.com/hi-jin/logseq-ask-pdf/raw/main/demo.gif)
> The demo video uses the paper [Frans, K., Park, S., Abbeel, P., & Levine, S. (2024). Unsupervised Zero-Shot Reinforcement Learning via Functional Reward Encodings.](https://arxiv.org/abs/2402.17135) as an example.

### Background

The 2nd-brain app Logseq is a powerful tool for knowledge management.  
It allows users to highlight the texts or images in the PDF and save them as blocks in Logseq.  
But, `Logseq lacks a feature that access the content of highlights directly`. (because, highlights are just simply a block of uuid pointing the text or image in the PDF)

Logseq Ask PDF is a plugin that `allows users to ask questions about PDF highlights directly within Logseq`.  
With this plugin, users don’t need to switch to the PDF file to find the highlights to ask questions.  
`This plugin also supports RAG (Retrieval Augmented Generation)` to answer questions based on the content of the PDF.

### Features

- Ask questions about PDF highlights directly within Logseq
- Supports asking both text and image highlights
- Use the entire PDF as context
- Seamless integration with Logseq’s UI
- Compatible with OpenAI API and local models that are OpenAI API-compatible

### Technical Details

- Typescript
- Langchain

### Links
- [Logseq Ask PDF on GitHub](https://github.com/hi-jin/logseq-ask-pdf)