# 🦉 Socrates — The Philosopher's Companion

A fully functional AI-powered philosophy chatbot built with Claude (Anthropic). Engages users in deep Socratic dialogue, debates, and philosophical inquiry across 8 branches of philosophy.

---

## 🌐 Live Demo

> [https://philosophy-chatbot.vercel.app](https://philosophy-chatbot.vercel.app)

---

## 🧠 Why Philosophy?

Philosophy is one of the richest topics for a conversational AI — it's open-ended, debate-driven, and never has a single "correct" answer. It lends itself naturally to the Socratic method: asking probing questions, exposing contradictions, and guiding the user toward deeper self-understanding. Every conversation is unique.

---

## ✨ Features

- **Socratic AI Persona** — the bot uses the Socratic method, cites Plato, Aristotle, Kant, Nietzsche, Sartre and more, and always ends with a probing question to deepen the dialogue
- **8 Philosophy Branches** — Ethics, Metaphysics, Epistemology, Existentialism, Political Philosophy, Philosophy of Mind, Aesthetics, Logic
- **Dynamic topic switching** — sidebar updates the bot's focus and quotes in real time
- **Starter prompts** — curated opening questions to reduce blank-page friction
- **Full conversation memory** — multi-turn dialogue maintained across the session
- **Polished UX states** — typing indicator, error state, empty state, smooth scroll
- **Responsive design** — works on mobile and desktop
- **Secure API** — Anthropic API key stored as a Vercel environment variable, never exposed in frontend code

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Vanilla HTML, CSS, JavaScript |
| Fonts | Playfair Display, EB Garamond (Google Fonts) |
| AI Model | Claude Sonnet (Anthropic API) |
| Backend | Vercel Serverless Function (`/api/chat.js`) |
| Deployment | Vercel |

---

## 📁 Project Structure

```
philosophy-chatbot/
├── index.html        # Full frontend — UI, styling, chat logic
└── api/
    └── chat.js       # Vercel serverless function — proxies Anthropic API securely
```

---

## 🚀 Running Locally

**1. Clone the repo**
```bash
git clone https://github.com/Akhil-Sheelam/philosophy-chatbot.git
cd philosophy-chatbot
```

**2. Install Vercel CLI**
```bash
npm install -g vercel
```

**3. Add your API key**

Create a `.env.local` file:
```
ANTHROPIC_API_KEY=sk-ant-your-key-here
```

**4. Run locally**
```bash
vercel dev
```

Open [http://localhost:3000](http://localhost:3000)

---

## 🔐 Environment Variables

| Variable | Description |
|---|---|
| `ANTHROPIC_API_KEY` | Your Anthropic API key from [console.anthropic.com](https://console.anthropic.com/keys) |

Set this in Vercel dashboard → Project Settings → Environment Variables.

---

## 💡 How I Built This

This project was built using **Claude (Anthropic)** as an AI coding assistant — in line with the assignment's encouragement to use AI tools effectively. The process involved:

1. Designing the topic and persona (Socratic philosopher)
2. Prompting Claude to generate the full UI with a specific aesthetic direction (parchment/ink editorial style)
3. Reviewing, testing, and iterating on the output
4. Architecting the secure API layer with a Vercel serverless function
5. Deploying and verifying the live build

The goal was not just to use AI, but to **direct it with precision** — making deliberate design choices, catching issues, and ensuring the final product feels purpose-built rather than generic.


## 👤 Author

**Akhil Sheelam**
- GitHub: [@Akhil-Sheelam](https://github.com/Akhil-Sheelam)

---

*"The unexamined life is not worth living." — Socrates*
