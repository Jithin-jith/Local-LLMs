# Local-LLMs
This repository contains implementations of how LLMs can be run locally using Ollama and LM Studio.

## What are Open LLM Models
Open LLM models are Large Language Models that are made publicly available, either fully open-source or with permissive licenses, allowing developers and organizations to:

- Use them for free (often commercially too)
- Fine-tune or adapt them for specific tasks
- Deploy them on their own hardware or in the cloud

## 🧪 Use Cases of Open LLMs
- Fine-tuning for custom chatbots or agents
- Embedding in private/local applications
- Educational use and research
- Evaluating fairness, bias, safety, etc.
- Building domain-specific assistants

## 🔍 What Makes an LLM “Open”?
An LLM is generally considered open if it meets most of these criteria:

|Criteria                |	Description                                                             |
|------------------------|--------------------------------------------------------------------------|
|✅ Weights Available    |	The trained model weights are freely downloadable                         |
|✅ Open License |	License allows commercial use, fine-tuning, and redistribution |
|✅ Code Access |	Training code, inference code, or config is shared|
|❌ Not Hosted Online |	Doesn’t require you to use the provider’s API (unlike GPT-4, Claude, etc.) |

---

## ✅ Top Options for Running LLMs Locally
🧠 1. Ollama
- URL: https://ollama.com
- Best for: Easiest local LLM setup with a CLI
- How it works: Pulls and runs models like llama3, mistral, gemma, phi3, etc.
- Pros:
    - One-line install
    - Offers advanced configuration options
    - Simple ollama run llama3 interface
    - GPU & CPU support
    - Mac, Linux, Windows (WSL)
- Cons:
    - Limited GUI; mainly CLI-based

💻 2. LM Studio
- URL: https://lmstudio.ai
- Best for: GUI-based chat with local models
- Pros:
    - Chat interface like ChatGPT
    - Drag-and-drop model loading from Hugging Face
    - Works on CPU & GPU
    - Prompt templates, multi-turn chat
    - Beautiful interface
    - Easy to run and switch models
    - Great for non-technical users
- Cons:
    - Slightly higher memory usage

⚡ 3. llama.cpp
- URL: https://github.com/ggerganov/llama.cpp
- Best for: Developers and CLI enthusiasts
- What it does: C++ implementation of LLaMA that runs on CPU/GPU using quantized models
- Use with: llama.cpp, text-generation-webui, koboldcpp, or ollama

---

## Licenses

### 🔍 1. MIT License (for software and models)

✅ **Overview**:  
One of the most permissive open-source licenses.  
Commonly used in traditional software, and some LLMs (e.g., Phi-2, GPT4All UI).

🔓 **You Can**:
- Use for personal or commercial projects  
- Modify and redistribute freely  
- Use in proprietary software  

🚫 **You Must**:
- Include the original license and copyright  

⚠️ **No Restrictions On**:
- Commercialization, hosting, or redistribution  

✅ **Best for**:  
Maximum flexibility; ideal if you want to build and sell apps

---

### 🦙 2. LLaMA License (Meta's custom license for LLaMA 2/3)

🔐 **Overview**:  
Not open-source in the traditional (OSI) sense.  
Research or commercial use allowed with conditions.

🔓 **You Can**:
- Use LLaMA for research and commercial use (subject to terms)  
- Fine-tune and host the model  

🚫 **You Cannot**:
- Use it in products competing with Meta  
- Remove Meta branding  
- Redistribute weights in some cases (especially modified ones)  

📝 **You Must**:
- Agree to Meta’s Acceptable Use Policy (AUP) and license agreement  
- Not violate restrictions like building harmful AI or competing products  

✅ **Best for**:  
Research projects, startups, and companies that don’t compete with Meta

---

### 🧠 3. Gemma License (Google’s license for Gemma)

📜 **Officially**: "Gemma Community License"

🔐 **Overview**:  
Not open-source.  
Allows personal, research, and commercial use — with limitations.

🔓 **You Can**:
- Use Gemma for research and commercial use  
- Run locally or in the cloud  

🚫 **You Cannot**:
- Use Gemma to build or improve competing LLMs  
- Use for training new foundational models  
- Redistribute modified versions of the weights  

📝 **You Must**:
- Follow Google’s terms, including ethical usage and branding  

✅ **Best for**:  
Developers and researchers who want to build apps or chatbots (but not base models)

