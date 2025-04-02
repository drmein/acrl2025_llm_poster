# Fine-Tuned, Low-Power and RAG(ged)

*Sustainable, privacy-preserving AI for libraries using minimal hardware*

## Project Overview

This repository contains resources from a project exploring how academic libraries can implement AI that aligns with our core values of privacy, sustainability, and institutional autonomy.

Using a Raspberry Pi and Retrieval-Augmented Generation (RAG), we've created a system that answers library FAQ questions with 80% less energy than cloud-based AI while keeping all data local. This approach allows libraries to provide AI assistance without compromising patron privacy or environmental responsibility.

### The Farm Metaphor

Just as we might choose a local sustainable farm over industrial factory farming, libraries can choose to run AI locally instead of relying on commercial cloud services:

| Local AI (Sustainable Farm) | Cloud AI (Industrial Factory) |
|----------------------------|------------------------------|
| Complete privacy control | Limited data control |
| Lower energy (5-15W) | Higher energy consumption |
| $50-150 one-time cost | Ongoing subscription costs |
| Slower (15-60+ seconds) | Faster responses (< 1 second) |

## Implementation Options

There are several approaches to implementing library AI, each with different tradeoffs:

1. **Small Local Model + RAG**
   - Hardware: Raspberry Pi 5 (8GB)
   - Model: SmolLM2-360M or similar
   - Privacy: Complete control
   - Response time: 15-60+ seconds
   - Cost: $50-150 one-time

2. **Medium Cloud-Hosted Model + RAG**
   - Deployment: Private cloud or institution's servers
   - Model: Mistral-7B or similar
   - Privacy: Good control
   - Response time: 1-3 seconds
   - Cost: $5-15/month

3. **Commercial API + RAG**
   - Deployment: Third-party API
   - Privacy: Limited control
   - Response time: < 1 second
   - Cost: Variable based on usage

## COMING SOON

This repository is being actively developed. Here's what you can expect in the coming weeks:

- **📚 Step-by-step implementation guides** for all approaches
- **🐍 Python scripts** for knowledge base preparation
- **🤖 RAG implementation** code for various models
- **⚡ Power consumption** measurement tools and results
- **📊 Performance benchmarks** across different models
- **🔧 Optimization techniques** for small models
- **🔗 Integration examples** with library chat services

*Full release planned for Summer 2025*

## Getting Started (Preliminary)

Until the full implementation guides are ready, here are some resources to begin exploring:

### Tools for Local LLM Exploration

- [Ollama](https://ollama.ai/) - Easy way to run LLMs locally (Mac/Linux)
- [LM Studio](https://lmstudio.ai/) - Desktop application to run models (Windows/Mac)
- [llama.cpp](https://github.com/ggerganov/llama.cpp) - Efficient LLM inference

### RAG Frameworks

- [LlamaIndex](https://www.llamaindex.ai/) - Framework for connecting LLMs with external data
- [LangChain](https://www.langchain.com/) - Building applications with LLMs through composability

### Small Models Worth Exploring

- [SmolLM](https://huggingface.co/smolmodels) - Efficient small language models
- [TinyLlama](https://github.com/jzhang38/TinyLlama) - Pretrained small language models
- [Phi-2](https://huggingface.co/microsoft/phi-2) - 2.7B parameter model with good performance

## The Power of RAG

Retrieval-Augmented Generation (RAG) significantly enhances the capabilities of small models by connecting them to your library's specific knowledge base.

**Example:**

Without RAG: *"Study rooms can typically be reserved online. Check your library's website."*

With RAG: *"Reserve study rooms at jwu-ri.libcal.com/allspaces. Only available to current JWU students, staff, or faculty. Reservations are forfeited after 15 minutes if no-show."*

## Skills Needed

This project involves various skills, but don't worry if you don't have all of them in-house:

### Technical Implementation
- Basic Python programming
- Command line familiarity
- Server/network configuration (for cloud options)

### Content Management
- FAQ organization
- Knowledge base preparation
- Quality assurance testing

*Projects can be implemented in collaboration with IT staff or consortium partners if in-house technical skills are limited.*

## Research & Background

This project builds on several areas of research:

- **Green AI:** Exploring energy-efficient approaches to AI deployment
- **Library Privacy:** Maintaining patron data sovereignty
- **Small Language Models:** Testing the capabilities of compact, efficient models
- **RAG vs. Fine-Tuning:** Comparing different approaches to knowledge integration

## Contact & Collaboration

Have questions or interested in collaborating? Reach out:

- David Meincke, Johnson & Wales University
- Email: david.meincke@jwu.edu
- ACRL 2025 Poster Session: Thursday, April 3rd, 2:00-3:45 PM

