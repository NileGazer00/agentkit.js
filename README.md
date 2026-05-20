<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&pause=1000&color=0A0A0A&center=true&vCenter=true&width=500&lines=agentkit.js;Build+AI+Agents+in+Plain+JS" alt="Typing SVG" />
</p>

<p align="center">
  <a href="https://github.com/NileGazer00/agentkit.js/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="MIT License" />
  </a>
  <a href="https://www.npmjs.com/package/agentkit">
    <img src="https://img.shields.io/npm/v/agentkit" alt="npm version" />
  </a>
  <a href="https://bundlephobia.com/package/agentkit">
    <img src="https://img.shields.io/bundlephobia/minzip/agentkit" alt="bundle size" />
  </a>
  <a href="https://github.com/NileGazer00/agentkit.js/stargazers">
    <img src="https://img.shields.io/github/stars/NileGazer00/agentkit.js?style=social" alt="GitHub stars" />
  </a>
  <a href="https://github.com/NileGazer00/agentkit.js/actions">
    <img src="https://img.shields.io/github/actions/workflow/status/NileGazer00/agentkit.js/ci.yml?branch=main" alt="CI" />
  </a>
</p>

<p align="center">
  <strong>Zero‑dependency AI agent framework for JavaScript</strong><br />
  ReAct reasoning • Tool calling • Memory • Streaming • Browser + Node
</p>

<p align="center">
  <a href="#-quick-start">Quick Start</a> •
  <a href="#-why-agentkitjs">Why AgentKit?</a> •
  <a href="#-architecture">Architecture</a> •
  <a href="#-complete-example">Example</a> •
  <a href="#-memory--tooling">Memory & Tooling</a> •
  <a href="#-live-demo--consulting">Consulting</a>
</p>

---

## 🌟 About AgentKit.js

**AgentKit.js** is a lightweight, zero‑dependency framework for building AI agents in plain JavaScript.  
It works in **Node.js** and **browsers**, supports multiple LLM providers (OpenAI, Anthropic, Google, Ollama, custom), and gives you full control with **no hidden abstractions**.

Inspired by the ReAct pattern, it lets you define tools as simple async functions, manage conversation memory, and stream output token by token — all in **~35 kB gzipped**.

---

## 📦 Install

```bash
npm install agentkit
⚡ Quick Start
javascript
import { Agent, tool } from 'agentkit'

// Define a tool
const calculator = tool({
  name: 'calculate',
  execute: async ({ expression }) => eval(expression)
})

// Create agent
const agent = new Agent({
  model: 'gpt-4o',
  tools: [calculator],
  strategy: 'react'
})

// Run
const result = await agent.run('What is 25 * 4 + 10?')
console.log(result.answer) // "110"
🚀 Why AgentKit.js?
Feature	agentkit.js	LangChain.js
Dependencies	0	48+
Bundle size	~35 kB	~800 kB
Browser support	✅ Yes	❌ No
TypeScript inference	✅ Full	⚠️ Partial
Streaming	✅ Native	Callbacks
Hidden abstractions	❌ None	Many
What you get:

🧠 ReAct reasoning – Thought → Action → Observation loop

🔧 Tool calling – Plain functions → auto‑schema tools

💾 Memory layers – Buffer, summary, vector memory built‑in

📡 Streaming – Async iterators for token‑by‑token output

🔀 Provider agnostic – OpenAI, Anthropic, Google, Ollama, or custom

🛡️ Guard rails – Max iterations, token budgets, permissions

🌐 Browser + Node – Same code everywhere

🧠 Architecture
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&pause=1000&color=0A0A0A&center=true&vCenter=true&width=500&lines=agentkit.js;Build+AI+Agents+in+Plain+JS" alt="Typing SVG" />
</p>

<p align="center">
  <a href="https://github.com/NileGazer00/agentkit.js/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="MIT License" />
  </a>
  <a href="https://www.npmjs.com/package/agentkit">
    <img src="https://img.shields.io/npm/v/agentkit" alt="npm version" />
  </a>
  <a href="https://bundlephobia.com/package/agentkit">
    <img src="https://img.shields.io/bundlephobia/minzip/agentkit" alt="bundle size" />
  </a>
  <a href="https://github.com/NileGazer00/agentkit.js/stargazers">
    <img src="https://img.shields.io/github/stars/NileGazer00/agentkit.js?style=social" alt="GitHub stars" />
  </a>
  <a href="https://github.com/NileGazer00/agentkit.js/actions">
    <img src="https://img.shields.io/github/actions/workflow/status/NileGazer00/agentkit.js/ci.yml?branch=main" alt="CI" />
  </a>
</p>

<p align="center">
  <strong>Zero‑dependency AI agent framework for JavaScript</strong><br />
  ReAct reasoning • Tool calling • Memory • Streaming • Browser + Node
</p>

<p align="center">
  <a href="#-quick-start">Quick Start</a> •
  <a href="#-why-agentkitjs">Why AgentKit?</a> •
  <a href="#-architecture">Architecture</a> •
  <a href="#-complete-example">Example</a> •
  <a href="#-memory--tooling">Memory & Tooling</a> •
  <a href="#-live-demo--consulting">Consulting</a>
</p>

---

## 🌟 About AgentKit.js

**AgentKit.js** is a lightweight, zero‑dependency framework for building AI agents in plain JavaScript.  
It works in **Node.js** and **browsers**, supports multiple LLM providers (OpenAI, Anthropic, Google, Ollama, custom), and gives you full control with **no hidden abstractions**.

Inspired by the ReAct pattern, it lets you define tools as simple async functions, manage conversation memory, and stream output token by token — all in **~35 kB gzipped**.

---

## 📦 Install

```bash
npm install agentkit
⚡ Quick Start
javascript
import { Agent, tool } from 'agentkit'

// Define a tool
const calculator = tool({
  name: 'calculate',
  execute: async ({ expression }) => eval(expression)
})

// Create agent
const agent = new Agent({
  model: 'gpt-4o',
  tools: [calculator],
  strategy: 'react'
})

// Run
const result = await agent.run('What is 25 * 4 + 10?')
console.log(result.answer) // "110"
🚀 Why AgentKit.js?
Feature	agentkit.js	LangChain.js
Dependencies	0	48+
Bundle size	~35 kB	~800 kB
Browser support	✅ Yes	❌ No
TypeScript inference	✅ Full	⚠️ Partial
Streaming	✅ Native	Callbacks
Hidden abstractions	❌ None	Many
What you get:

🧠 ReAct reasoning – Thought → Action → Observation loop

🔧 Tool calling – Plain functions → auto‑schema tools

💾 Memory layers – Buffer, summary, vector memory built‑in

📡 Streaming – Async iterators for token‑by‑token output

🔀 Provider agnostic – OpenAI, Anthropic, Google, Ollama, or custom

🛡️ Guard rails – Max iterations, token budgets, permissions

🌐 Browser + Node – Same code everywhere

🧠 Architecture
















The agent continues the cycle until a final answer is produced or the maximum iteration limit is reached.

🔧 Complete Example: Web Search Agent
javascript
import { Agent, tool } from 'agentkit'

const webSearch = tool({
  name: 'web_search',
  description: 'Search the web for current information',
  parameters: {
    query: { type: 'string', description: 'Search query' }
  },
  execute: async ({ query }) => {
    const res = await fetch(`https://api.serper.dev/search?q=${query}`, {
      headers: { 'X-API-KEY': process.env.SERPER_API_KEY }
    });
    const data = await res.json();
    return data.organic.map(o => o.snippet).join('\n');
  }
});

const agent = new Agent({
  model: 'gpt-4o',
  tools: [webSearch],
  strategy: 'react',
  maxIterations: 5,
  tokenBudget: 4000
});

const result = await agent.run('What are the top 3 AI frameworks in 2026?');
console.log(result.answer);
🧩 Memory & Tooling
Buffer memory (keeps last N messages):

javascript
import { Agent, BufferMemory } from 'agentkit'
const memory = new BufferMemory({ limit: 10 })
const agent = new Agent({ model: 'gpt-4o', memory, tools: [...] })
Summary memory (auto‑compress history):

javascript
import { SummaryMemory } from 'agentkit'
const memory = new SummaryMemory({ threshold: 20, summarizerModel: 'gpt-3.5-turbo' })
🌍 Live Demo & Consulting
Try it live: agentkit.js demo

I'm Nile Gazer, creator of AgentKit.js. I build production‑grade AI agent systems for startups and enterprises.
Hire me for custom agents, RAG pipelines, LLM integrations, or full‑stack AI products.

📧 Email: jusspound@gmail.com

🌐 Portfolio: nilegazer00.github.io

🐙 GitHub: NileGazer00

🤝 Contributing
We welcome contributions! Please read CONTRIBUTING.md to get started.
Open an issue first to discuss significant changes.

📄 License
Distributed under the MIT License. See LICENSE for more information.

<p align="center"> <strong>⭐ Star this repo to support the project and help others discover AgentKit.js ⭐</strong> </p> ```















