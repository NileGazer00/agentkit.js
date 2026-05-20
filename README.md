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
  <a href="https://github.com/NileGazer00/agentkit.js">
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
  <a href="#-live-demo--consulting">Consulting</a>
</p>

---

## 📦 Install

```bash
npm install agentkit
##⚡ Quick Start
import { Agent, tool } from 'agentkit'

// 1️⃣ Define a tool
const calculator = tool({
  name: 'calculate',
  execute: async ({ expression }) => eval(expression)
})

// 2️⃣ Create an agent
const agent = new Agent({
  model: 'gpt-4o',
  tools: [calculator],
  strategy: 'react'
})

// 3️⃣ Run it
const result = await agent.run('What is 25 * 4 + 10?')
console.log(result.answer) // "110"
