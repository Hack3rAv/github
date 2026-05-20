Copy

On this page

1.  [Get Started](/docs/get-started)

🦥Unsloth Docs
==============

Unsloth is an open-source framework for running and training LLMs.

Unsloth lets you run and train AI models on your own local hardware via an open-source UI.

Our docs will guide you through running & training your own LLM locally.

[Get started](/docs/new/studio) [Our GitHub](https://github.com/unslothai/unsloth)

[](/docs/models/qwen3.6#mtp-guide)

![Cover](./assets/image)

**Qwen3.6 MTP**

Run Qwen3.6 ~2x faster with no accuracy loss.

[](/docs/basics/api)

![Cover](./assets/image)

**Unsloth API endpoint**

Run inference with Unsloth via our new API.

[](/docs/models/gemma-4)

![Cover](./assets/image)

**Google Gemma 4**

Run and train Google's new Gemma 4 models!

[](/docs/models/nemotron-3-nano-omni)

![Cover](./assets/image)

**NVIDIA Nemotron 3 Omni**

Run the strongest 30B omni locally.

[](/docs/new/studio)

![Cover](./assets/image)

**Introducing Unsloth Studio**

New open, no-code UI to train and run LLMs.

[](/docs/models/qwen3.6)

![Cover](./assets/image)

**Qwen3.6**

The new Qwen3.6-27B model is here!

[🧬Fine-tuning Guide](/docs/get-started/fine-tuning-llms-guide)[📒Unsloth Notebooks](/docs/get-started/unsloth-notebooks)

[🔮All Our Models](/docs/get-started/unsloth-model-catalog)[🚀Complete LLM Directory](/docs/models/tutorials)

### 

[](#why-unsloth)

🦥 Why Unsloth?

*   We directly collab with teams behind [gpt-oss](https://docs.unsloth.ai/new/gpt-oss-how-to-run-and-fine-tune#unsloth-fixes-for-gpt-oss), [Qwen3](https://www.reddit.com/r/LocalLLaMA/comments/1kaodxu/qwen3_unsloth_dynamic_ggufs_128k_context_bug_fixes/), [Llama 4](https://github.com/ggml-org/llama.cpp/pull/12889), [Mistral](https://huggingface.co/mistralai/Mistral-Medium-3.5-128B/discussions/18), [Gemma 1-3](https://news.ycombinator.com/item?id=39671146) and [Phi-4](https://unsloth.ai/blog/phi4), where we’ve **fixed critical bugs** that greatly improved model accuracy. Andrej Karpathy for example has [praised our work](https://x.com/karpathy/status/1765473722985771335).
    
*   Unsloth streamlines local training, inference, data, and deployment
    
*   Unsloth supports inference and training for 500+ models: [vision](/docs/basics/vision-fine-tuning), [TTS](/docs/basics/text-to-speech-tts-fine-tuning), [embedding](/docs/basics/embedding-finetuning), [RL](/docs/get-started/reinforcement-learning-rl-guide)
    

### 

[](#features)

⭐ Features

Unsloth lets you run and train models for text, [audio](https://unsloth.ai/docs/basics/text-to-speech-tts-fine-tuning), [embedding](https://unsloth.ai/docs/new/embedding-finetuning), [vision](https://unsloth.ai/docs/basics/vision-fine-tuning) and more. Unsloth provides many key features for both inference and training:

#### 

[](#inference)

Inference

*   Search + download + run any model like GGUFs, LoRA adapters, safetensors.
    
*   [Self-healing tool calling](/docs/new/studio/chat#auto-healing-tool-calling) / web search and call OpenAI-compatible APIs.
    
*   [Auto inference parameter](/docs/new/studio/chat#auto-parameter-tuning) tuning and edit chat templates.
    
*   [Export or save](/docs/new/studio/export) your model to GGUF, 16-bit safetensor etc.
    
*   [Compare outputs](/docs/new/studio/chat#model-arena) with two different model side by side.
    

#### 

[](#training)

Training

*   Train and [RL](/docs/get-started/reinforcement-learning-rl-guide) 500+ models ~2x faster with ~70% less VRAM (no accuracy loss)
    
*   Supports full fine-tuning, pre-training, 4-bit, 16-bit and FP8 training.
    
*   [Auto-create datasets](/docs/new/studio/data-recipe) from PDF, CSV, DOCX files. Edit data in a visual node workflow.
    
*   Observability: Monitor training live, track loss, GPU usage, customize graphs
    
*   Most efficient [**reinforcement learning**](/docs/get-started/reinforcement-learning-rl-guide) library, using 80% less VRAM for GRPO, [FP8](/docs/get-started/reinforcement-learning-rl-guide/fp8-reinforcement-learning) etc.
    
*   [Multi-GPU](/docs/basics/multi-gpu-training-with-unsloth) works but a much better version is coming!
    

### 

[](#quickstart)

Quickstart

Unsloth supports MacOS, Linux, [Windows](/docs/get-started/install/windows-installation), [NVIDIA](/docs/get-started/install/pip-install), Intel and CPU setups. See: [Unsloth Requirements](/docs/get-started/fine-tuning-for-beginners/unsloth-requirements). Use the same commands to update:

#### 

[](#macos-linux-wsl)

**MacOS, Linux, WSL:**

#### 

[](#windows-powershell)

**Windows PowerShell:**

#### 

[](#docker)

Docker

Use our official **Docker image**: [`unsloth/unsloth`](https://hub.docker.com/r/unsloth/unsloth) which currently works for Windows, WSL and Linux. MacOS support coming soon.

#### 

[](#launch-unsloth)

Launch Unsloth

### 

[](#what-is-fine-tuning-and-rl-why)

What is Fine-tuning and RL? Why?

[**Fine-tuning** an LLM](/docs/get-started/fine-tuning-llms-guide) customizes its behavior, enhances domain knowledge, and optimizes performance for specific tasks. By fine-tuning a pre-trained model (e.g. Llama-3.1-8B) on a dataset, you can:

*   **Update Knowledge**: Introduce new domain-specific information.
    
*   **Customize Behavior**: Adjust the model’s tone, personality, or response style.
    
*   **Optimize for Tasks**: Improve accuracy and relevance for specific use cases.
    

[**Reinforcement Learning (RL)**](/docs/get-started/reinforcement-learning-rl-guide) is where an "agent" learns to make decisions by interacting with an environment and receiving **feedback** in the form of **rewards** or **penalties**.

*   **Action:** What the model generates (e.g. a sentence).
    
*   **Reward:** A signal indicating how good or bad the model's action was (e.g. did the response follow instructions? was it helpful?).
    
*   **Environment:** The scenario or task the model is working on (e.g. answering a user’s question).
    

**Example fine-tuning or RL use-cases**:

*   Enables LLMs to predict if a headline impacts a company positively or negatively.
    
*   Can use historical customer interactions for more accurate and custom responses.
    
*   Fine-tune LLM on legal texts for contract analysis, case law research, and compliance.
    

You can think of a fine-tuned model as a specialized agent designed to do specific tasks more effectively and efficiently. **Fine-tuning can replicate all of RAG's capabilities**, but not vice versa.

[🤔FAQ + Is Fine-tuning Right For Me?](/docs/get-started/fine-tuning-for-beginners/faq-+-is-fine-tuning-right-for-me)[🖥️Inference & Deployment](/docs/basics/inference-and-deployment)

[💡Reinforcement Learning Guide](/docs/get-started/reinforcement-learning-rl-guide)[🦥Dynamic 2.0 GGUFs](/docs/basics/unsloth-dynamic-2.0-ggufs)

![](./assets/image)

[NextBeginner? Start here!](/docs/get-started/fine-tuning-for-beginners)

Last updated 12 hours ago

Was this helpful?
