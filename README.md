# 🚨 VibeCheck AI | Dating Intelligence Agent

A context-aware, highly conversational AI Agent built on **n8n** that serves as a protective, witty dating profile critic and message analyzer. Designed to run as a lightweight web application, it interprets dating app bios, prompts, and chat logs to evaluate effort levels, identify red flags, and generate high-value conversational counter-strikes.

---

## 🚀 Live Demo
Try out the web interface live here: 
👉 `https://YOUR_GITHUB_USERNAME.github.io/project-cartier/` *(Replace with your actual live GitHub Pages URL)*

---

## 🛠️ Technical Architecture & Stack
This project bridges a visual node-based backend automation workflow with a clean, responsive frontend web interface.

*   **Backend Orchestration:** `n8n` (Advanced AI Workflow Framework)
*   **LLM Core:** `OpenAI GPT-4o` / `Claude 3.5 Sonnet` (via Chat Model Node)
*   **Memory Layer:** `Simple Memory` node (maintains continuous conversational context across multiple text updates)
*   **Trigger Mechanism:** `Chat Trigger` configured as a Webhook Public Production Endpoint
*   **Frontend Interface:** Single-file custom HTML5/CSS3 application styled with native iOS system font stacks and embedded using the official `n8n Chat CDN` widget.

---

## 🧠 System Prompt Core Logic
The underlying AI Agent is governed by a strict structured routing prompt that ensures it dynamically shifts between friendly banter and structured evaluation:

1.  **Casual Conversations:** Detects if the user is introducing themselves or making casual conversation, adopting a supportive, "best-friend" persona.
2.  **The Vibe Check:** Rates the profile's effort level from 1 to 10 and provides a sharp one-sentence summary.
3.  **Red Flags & Subtext:** Leverages advanced reasoning to extract the hidden meaning behind low-effort or emotionally unavailable bio clichés.
4.  **Green Flags:** Searches for authentic green flags (returning a custom `Error 404` string if none are present).
5.  **The Counter-Strike:** Generates dual response paths—**The Shutdown** (for quick dismissals) and **The Hook** (to test the waters playfully).

---

## 📁 Repository Structure
```text
├── index.html       # The frontend interface utilizing n8n embedded chat CDN
├── README.md        # Project documentation and architecture details
└── workflow.json    # Exported n8n production workflow logic (ready for import)
