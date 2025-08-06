# 🧠 What is Ollama?

**Ollama** is a powerful **command-line tool and runtime** that makes it super easy to run and manage large language models (LLMs) locally on your machine.

> Think of it like **Docker**, but for **LLMs**.

Instead of worrying about downloading weights, converting formats, setting up tokenizers, or writing inference code, **Ollama wraps all of that into a single smooth experience**.

---

# ✅ What Can You Do with Ollama?

- 🏃‍♂️ **Run models** like **LLaMA 2**, **Mistral**, **Gemma**, **Phi**, **Codellama**, **OpenHermes**, **Neural Chat**, and more **locally**.
- 🧩 **Customize models** using `Modelfiles`. - https://github.com/ollama/ollama/blob/main/docs/modelfile.md
- 💬 **Chat** with models from your **terminal** or **build apps** using the **Ollama API** - https://github.com/ollama/ollama/blob/main/docs/api.md.
- 🛠️ **Fine-tune** or **personalize** models.


# 🛠️ Ollama CLI: Essential Commands

## 📋 General Commands

/?, /help  
> Show list of all available commands

/version  
> Display the Ollama CLI version

/models  
> List all models currently pulled on your machine

/run <model-name>  
> Run a model and start interactive chat session  
> Example: `ollama run mistral`

/pull <model-name>  
> Download a model from the Ollama model registry  
> Example: `ollama pull llama2`

/push <model-name>  
> Push your custom model to Ollama registry (if you have permissions)

/list  
> Alias for `/models` – shows all local models

/show <model-name>  
> Show details about a specific model (like size, architecture)

/show info  
> Show general info about the running model session

/show system  
> Show system message set for the current model

/help  
> Display usage help for any command

/exit or Ctrl+C  
> Exit from chat or interactive mode

## ⚙️ Modelfile & Custom Models

/create <model-name>  
> Create a new model from a `Modelfile` in current directory  
> Example: `ollama create my-custom-model`

## 🔁 System Control

/stop <model-name>  
> Stop a running model process  
> Example: `ollama stop llama2`

/delete <model-name>  
> Delete a model from your local system  
> Example: `ollama delete mistral`

## 🌐 REST API (Local Server)

ollama serve  
> Starts the Ollama server to access via REST API (`http://localhost:11434`)

## 📜 Example: Using with curl

```bash
curl http://localhost:11434/api/generate -d '{
  "model": "mistral",
  "prompt": "Explain Quantum Physics simply"
}'
