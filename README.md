# Giulio Leone

**AI Engineer & Software Architect** — Building intelligent systems and contributing to the open-source AI ecosystem.

---

## 🔧 Open-Source Contributions

Active contributor to foundational AI infrastructure projects. Focused on reliability, correctness, and developer experience.

### [Vercel AI SDK](https://github.com/vercel/ai) — `30 PRs`

The most widely adopted TypeScript toolkit for building AI applications. Key contributions:

| Area | PR | Impact |
|------|----|--------|
| **Error Handling** | [#12928](https://github.com/vercel/ai/pull/12928) | Fixed `generateText()` silently swallowing `AbortError` in multi-step tool loops |
| **Stream Reliability** | [#12929](https://github.com/vercel/ai/pull/12929) | Fixed "Controller is already closed" crash during async tool execution |
| **React Hooks** | [#12930](https://github.com/vercel/ai/pull/12930) | Fixed `useChat` stale transport body — reported by [Matt Pocock](https://github.com/mattpocock) |
| **Provider: Anthropic** | [#12931](https://github.com/vercel/ai/pull/12931) | Fixed extended thinking + multi-step tool use crash (14 👍) |
| **Observability** | [#12932](https://github.com/vercel/ai/pull/12932), [#12933](https://github.com/vercel/ai/pull/12933) | Added missing telemetry attributes for token usage and tool calls |
| **Provider: OpenAI** | [#12937](https://github.com/vercel/ai/pull/12937) | Responses API stream errors now surface proper `APICallError` with status codes |
| **DX** | [#12938](https://github.com/vercel/ai/pull/12938) | Partial streamed messages preserved on `useChat` error instead of being lost |
| **Provider: Azure** | [#12939](https://github.com/vercel/ai/pull/12939), [#12941](https://github.com/vercel/ai/pull/12941) | Fixed `repairToolCall` not invoked + reasoning ID rejection with `store:false` |
| **Provider: Google** | [#12944](https://github.com/vercel/ai/pull/12944) | Fixed Gemini enum-only schemas missing required `type` field |
| **Provider: Bedrock** | [#12943](https://github.com/vercel/ai/pull/12943) | Fixed cross-region inference prefix breaking embedding model detection |
| **Interop** | [#12940](https://github.com/vercel/ai/pull/12940), [#12942](https://github.com/vercel/ai/pull/12942) | OpenAI-compatible audio/video support + missing `type:object` in tool schemas |
| **RFC Compliance** | [#12945](https://github.com/vercel/ai/pull/12945) | User-Agent RFC 9110 violation causing Azure 400 errors on Bun |
| **Integrations** | [#12946](https://github.com/vercel/ai/pull/12946) | LangChain HITL tool call ID mismatch breaking human-in-the-loop |
| **Gateway** | [#12935](https://github.com/vercel/ai/pull/12935), [#12936](https://github.com/vercel/ai/pull/12936) | Image generation cost aggregation + file chunk metadata preservation |

### [Model Context Protocol SDK](https://github.com/modelcontextprotocol/typescript-sdk) — `6 PRs`

The official TypeScript SDK for MCP, the open standard for AI tool integration.

- [#1598](https://github.com/modelcontextprotocol/typescript-sdk/pull/1598) — `server.tool()` silently dropped JSON Schema when passed raw objects instead of Zod
- [#1599](https://github.com/modelcontextprotocol/typescript-sdk/pull/1599) — OAuth token exchange failed with URL-encoded responses (GitHub compatibility)
- [#1600](https://github.com/modelcontextprotocol/typescript-sdk/pull/1600) — `ResourceSchema` missing `size` field defined in the MCP specification
- [#1601](https://github.com/modelcontextprotocol/typescript-sdk/pull/1601) — OAuth scope overwrite prevented progressive authorization
- [#1602](https://github.com/modelcontextprotocol/typescript-sdk/pull/1602) — Server re-registered capabilities on every connection
- [#1603](https://github.com/modelcontextprotocol/typescript-sdk/pull/1603) — `z.object()` schemas silently stripped all tool arguments

### [AG-UI Protocol](https://github.com/ag-ui-protocol/ag-ui) — `4 PRs`

The emerging open protocol for Agent-to-UI communication.

- [#1199](https://github.com/ag-ui-protocol/ag-ui/pull/1199) — `process.env` references crashed in browser environments
- [#1200](https://github.com/ag-ui-protocol/ag-ui/pull/1200) — Python SDK `ReasoningMessageRole` was `"assistant"` instead of `"reasoning"`
- [#1201](https://github.com/ag-ui-protocol/ag-ui/pull/1201) — `Tool.parameters` optionality mismatch between TypeScript and Python SDKs
- [#1202](https://github.com/ag-ui-protocol/ag-ui/pull/1202) — Mastra integration `JSON.parse` crash on malformed working memory

### [LangChain.js](https://github.com/langchain-ai/langchainjs) — `1 PR`

- [#10188](https://github.com/langchain-ai/langchainjs/pull/10188) — `ChatGoogleGenerativeAI` crashed with undefined message when Google blocked content (9 👍)

### [CopilotKit](https://github.com/CopilotKit/CopilotKit) — `2 PRs`

- [#3314](https://github.com/CopilotKit/CopilotKit/pull/3314) — Global KaTeX CSS import broke Next.js builds with `optimizeCss` (7 👍, `help wanted`)
- [#3315](https://github.com/CopilotKit/CopilotKit/pull/3315) — Non-object tool arguments from LLMs caused permanent Anthropic 400 errors

---

## 🏗️ Personal Projects

| Project | Description |
|---------|-------------|
| **OneGenUI** | Modular AI-native UI framework with deep research, document parsing, MCP integration, and vector search |
| **OneAgent** | Autonomous agent framework with composable hooks and skill system |
| **CoachOne** | AI coaching platform — full-stack TypeScript with domain-driven backend architecture |
| **Agent Browser** | Browser automation powered by AI agents |
| **VS Code Agent Skills** | Hypothesis-driven debugging and self-evolving skills for VS Code Copilot |

---

## 💡 Focus Areas

- **AI SDK Infrastructure** — Error handling, streaming reliability, provider compatibility
- **Agent Protocols** — MCP, AG-UI, tool calling standards
- **Full-Stack AI Applications** — React/Next.js + LLM integration patterns
- **Software Architecture** — Hexagonal architecture, DDD, SOLID principles

---

<p align="center">
  <a href="https://github.com/giulio-leone?tab=repositories">Repositories</a> ·
  <a href="https://github.com/pulls?q=is%3Apr+author%3Agiulio-leone+is%3Aopen">Open PRs</a>
</p>
