# Working with AI
A collection of AI related...concepts, tools, etc.

## Terms

| Term | Used for | Consumed by | See also | Ref |
|------|----------|-------------|----------|-----|
| AGENTS.md | Repository-level instructions for AI agents | Codex, Cursor, Claude Code | Harness, SKILLS.md, RULES.md / .cursorrules | [OpenAI Codex — AGENTS.md](https://developers.openai.com/codex/guides/agents-md/) |
| llms.txt | Standardized site/repo info for LLMs at inference time | LLMs, crawlers, IDE plugins | Context engineering, RAG | [llmstxt.org](https://llmstxt.org/) |
| SKILLS.md | Reusable agent skill definitions | Codex, Cursor | AGENTS.md, Harness | [agentskills.io](https://agentskills.io/home) |
| RULES.md / .cursorrules | Project coding rules and conventions for AI assistants | Cursor | AGENTS.md, Prompt engineering | [Cursor — Rules](https://docs.cursor.com/context/rules) |
| MCP (Model Context Protocol) | Connecting models to external tools and data | Claude Desktop, Cursor, IDEs | Tool use / function calling, Harness | [modelcontextprotocol.io](https://modelcontextprotocol.io/) |
| Prompt Engineering | Crafting effective prompts (structure, examples, roles) | Developers, chat UIs | Few-shot prompting, CoT, System prompt | [Anthropic — Prompt engineering](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview) |
| Context Engineering | Designing what information reaches the model | Agent frameworks, developers | llms.txt, RAG, Memory | [context-engineering.md](context-engineering.md) |
| RAG (Retrieval-Augmented Generation) | Grounding answers with retrieved documents | Agent frameworks, search apps | Context engineering, llms.txt | [Wikipedia — RAG](https://en.wikipedia.org/wiki/Retrieval-augmented_generation) |
| Agentic Coding | Using AI agents for software development | Developers | Harness, Tool use | [MIT — Agentic Coding](https://youtu.be/sTdz6PZoAnw?si=zGJmjsFVVXxzIeHl) |
| Harness | Orchestration that turns an LLM into an agent (tools, loops, memory) | Agent frameworks | LLM, MCP, Tool use | [LangChain — harness](https://blog.langchain.com/the-anatomy-of-an-agent-harness/) |
| Chain-of-Thought (CoT) | Prompting the model to reason step-by-step | LLMs | Prompt engineering, Few-shot | [Wei et al. — CoT](https://arxiv.org/abs/2201.11903) |
| Few-shot Prompting | Providing in-prompt examples to shape output | LLMs | Prompt engineering, CoT | [Anthropic — Prompting](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview) |
| Hallucination | Plausible but incorrect model output | Developers (mitigation) | RAG, Context engineering | [Wikipedia — AI hallucination](https://en.wikipedia.org/wiki/Hallucination_(artificial_intelligence)) |
| Tool use / function calling | Letting models invoke tools or APIs | LLMs, agent harnesses | MCP, Harness | [OpenAI — Function calling](https://platform.openai.com/docs/guides/function-calling) |
| System prompt | Instructions that set behavior and persona (often hidden) | LLMs | Prompt engineering, RULES.md / .cursorrules | [OpenAI — Prompt engineering](https://platform.openai.com/docs/guides/prompt-engineering) |

## Refs
- `Harness + LLM = Agent` 
  - [Langchain blogpost on harness](https://blog.langchain.com/the-anatomy-of-an-agent-harness/)
- [MIT, The Missing Semester, Agentic Coding](https://youtu.be/sTdz6PZoAnw?si=zGJmjsFVVXxzIeHl)
- [Skills](https://agentskills.io/home)