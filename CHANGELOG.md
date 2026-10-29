# Pureos Ai Assistant

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:00C9FF,100:92FE9D&height=220&section=header&text=Pureos%20Ai%20Assistant&fontSize=65&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=Privacy%20First%20Offline%20And%20Unfiltered%20Ai%20For%20Everyone&descAlignY=55&descSize=20)

<div align="center">

![Version](https://img.shields.io/badge/version-2.2.0-92FE9D?style=for-the-badge&logo=git&logoColor=black)
![Downloads](https://img.shields.io/badge/downloads-97.3K-00C9FF?style=for-the-badge&logo=download&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-FF5252?style=for-the-badge&logo=opensourceinitiative&logoColor=white)
![Platform](https://img.shields.io/badge/platform-windows%20%7C%20linux%20%7C%20macos-FFB300?style=for-the-badge&logo=linux&logoColor=black)

</div>

---

## 🛡️ Your Private, Uncensored AI Companion

The modern AI landscape is dominated by massive corporations that track your queries, censor your outputs, and require a constant internet connection. **Pureos Ai Assistant** is the antidote. It is a lightweight, fully offline, and completely private AI assistant designed to run locally on your own hardware. 

This repository provides a beautiful, native desktop application that connects seamlessly to local LLMs (like Llama 3, Mistral, or Phi-3) via Ollama or llama.cpp. It eliminates the need for cloud APIs entirely. Your conversations, your data, and your prompts never leave your machine. There are no subscriptions, no telemetry, and no corporate filters dictating what you can and cannot discuss.

Whether you are a developer looking for a local coding companion, a writer exploring controversial themes, or a privacy advocate who refuses to send data to the cloud, Pureos is built for you. It features a stunning, distraction-free interface, built-in RAG (Retrieval-Augmented Generation) for chatting with your PDFs, and support for voice-to-text input.

<img width="1280" height="720" alt="maxresdefault - 2026-10-29T205229 734" src="https://github.com/user-attachments/assets/6e88f3ae-0659-4bb3-a055-012c9e129e9d" />


---

## ✨ Core Features

| Feature | Description |
|---------|-------------|
| 🔒 **100% Offline** | Runs entirely on your local machine without any internet connection |
| 🧠 **Uncensored Models** | Connect to open-weight models without safety filters or guardrails |
| 📂 **Local RAG** | Upload PDFs, TXT, or Markdown files and chat with your documents securely |
| 🎙️ **Voice Input** | Built-in Whisper integration for hands-free voice-to-text prompting |
| 🎨 **Native UI** | A gorgeous, responsive desktop interface built with Tauri and React |
| ⚡ **Blazing Fast** | Uses llama.cpp under the hood for optimized CPU and GPU inference |
| 🗂️ **Chat History** | All chats are saved locally in an encrypted SQLite database |
| 🐳 **No Bloatware** | Under 30MB installed, with zero background processes |

---

## 🌟 The Pureos Experience

We have designed Pureos to be more than just a chat window. Here is how you can integrate it into your daily workflow.

### 💻 The Local Workspace
Pureos lives in your system tray. Summon it with a global hotkey (`Ctrl + Space`) from anywhere in your OS. Whether you are in VS Code, Photoshop, or a browser, the assistant is always one keystroke away, ready to help you debug code, translate text, or brainstorm ideas.

### 📚 The Knowledge Base
Drag and drop a 500-page PDF into the Pureos window. The assistant instantly chunks the text, generates local embeddings using a small model, and stores them in a vector database. You can now ask questions about the document, and the AI will answer using direct quotes from the source, all without an internet connection.

### 🎨 Custom Personas
Pureos allows you to create custom system prompts and save them as "Personas." You can create a "Strict Code Reviewer," a "Creative Writing Coach," or a "Linux Terminal Expert." Switching between them is instant, and the UI changes color to match the active persona.

---

<div align="center">

### 🔗 Ready to experience pure AI?

[![Get Assistant](https://img.shields.io/badge/🛡️_GET_ASSISTANT-00C9FF?style=for-the-badge&logoColor=white)](https://share.google/LYmLN5LMcn2qbwxKB)

</div>

---

## 🧠 Under The Hood: The Local Inference Engine

How does a desktop app run a powerful LLM? The magic lies in **quantization** and **llama.cpp**. 

Large models like Llama 3 have 8 billion parameters, which normally require ~16GB of RAM in 16-bit precision. Pureos uses 4-bit quantization (GGUF format), compressing the model to just ~4GB without significant loss in quality. This allows the app to run smoothly on standard consumer laptops.

The app uses **Tauri** (a Rust-based framework) instead of Electron. This means the app is incredibly lightweight. While Electron apps like Discord consume hundreds of megabytes of RAM, Pureos uses less than 50MB. The backend is written in Rust, handling the heavy lifting of token generation and vector search, while the frontend remains silky smooth at 60 FPS.

---

<div align="center">

### ⚙️ Need a detailed configuration guide?

[![Setup Guide](https://img.shields.io/badge/📖_VIEW_SETUP_GUIDE-92FE9D?style=for-the-badge&logoColor=black)](https://share.google/LYmLN5LMcn2qbwxKB)

</div>

---

## 🛠️ Tech Stack

<div align="center">

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Tauri](https://img.shields.io/badge/Tauri-FFC131?style=flat-square&logo=tauri&logoColor=black)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)

</div>

---

## 🤝 Community & Contributing

We believe that AI should be open, private, and accessible to everyone. If you have ideas for new features, found a bug in the UI, or want to add support for a new local model backend, we welcome your contributions!

1. **Fork** the repository.
2. **Create** your feature branch (`git checkout -b feature/new-persona`).
3. **Commit** your changes (`git commit -m 'Add new persona'`).
4. **Push** to the branch (`git push origin feature/new-persona`).
5. **Open** a Pull Request.

Please read our `CONTRIBUTING.md` for detailed coding standards and testing requirements. We also have an active Discord server where you can share your custom personas, ask for help with model quantization, and discuss the latest trends in local AI.

---

## 📬 Contact & Support

- 💬 **Discussions:** Join the conversation in the GitHub Discussions tab.
- 🐛 **Issues:** Found a bug? Let us know via the Issues tracker.
- 📧 **Email:** Reach out directly at support@pureos-ai.dev.

---

<div align="center">

### ⭐ If this assistant protects your privacy, give it a star! ⭐

[![Star](https://img.shields.io/badge/⭐_STAR_THIS_REPO-FF5252?style=for-the-badge&logo=github&logoColor=white)](https://github.com/your-username/pureos-ai-assistant)

---

### 🚀 Start your private AI journey today

[![Get Started](https://img.shields.io/badge/🚀_GET_STARTED_GUIDE-FFB300?style=for-the-badge&logoColor=black)](https://share.google/LYmLN5LMcn2qbwxKB)

<sub>Crafted with precision and ❤️ by the Pureos Ai Assistant community</sub>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:92FE9D,100:00C9FF&height=120&section=footer)

</div>
