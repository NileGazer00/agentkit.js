# agentkit.js

> Zero-dependency AI agent framework for JavaScript

[![MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE) [![Zero Deps](https://img.shields.io/badge/dependencies-0-green.svg)]()

## Install

    npm install agentkit

## Quick Start

    import { Agent, tool } from 'agentkit'
    const agent = new Agent({ model: 'gpt-4o', tools: [myTool] })
    const result = await agent.run('Your prompt here')

## Features

- ReAct Reasoning
- Tool Calling
- Memory Layers
- Streaming
- Provider Agnostic
- Guard Rails
- Browser + Node
- TypeScript First

## Author

**Nile Gazer** - jusspound@gmail.com
[Portfolio](https://nilegazer00.github.io) | [GitHub](https://github.com/NileGazer00)

## License

MIT
