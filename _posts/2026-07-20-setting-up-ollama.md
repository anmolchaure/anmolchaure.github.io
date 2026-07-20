---
title: "Running a Local LLM with Ollama"
date: 2026-07-20
categories:
  - notes
tags:
  - llm
  - ollama
  - environmental-modelling
toc: true
---

## Why run an LLM locally

Running a model locally gives you control, privacy,
and offline operationno per-token cost and no data leaving
the device.

## Hardware constraints

I have a CPU-only machine with 6GB RAM, so it will be best to stick to 3B-parameter models.
A 3B model at Q4 quantization is roughly 2GB, which leaves headroom
for my operating system.

## Installing Ollama on Ubuntu

```bash
curl -fsSL https://ollama.com/install.sh | sh
ollama run llama3.2:3b
```

---