# Self-Hosted AI Agents

A curated list of open source AI agents you can run on your own hardware. Every entry here is
self-hosted: you install it on a machine you control, it keeps its data there, and most of them
work with local models through Ollama, llama.cpp or any OpenAI-compatible endpoint, so nothing
has to leave the house.

The list covers personal assistants that live in your chat apps, coding agents, research and
browser agents, visual workflow builders, chat interfaces with tool use, voice agents, the
frameworks people build agents with, and the runtimes that serve the models. Archived projects
are left out. Star counts are not listed because they go stale; each link goes to the live repo.

## Contents

- [Personal assistants and autonomous agents](#personal-assistants-and-autonomous-agents)
- [Coding agents](#coding-agents)
- [Research agents](#research-agents)
- [Browser agents](#browser-agents)
- [Visual builders and workflow platforms](#visual-builders-and-workflow-platforms)
- [Chat interfaces with agents and tools](#chat-interfaces-with-agents-and-tools)
- [Voice agents](#voice-agents)
- [Agent frameworks](#agent-frameworks)
- [Memory for agents](#memory-for-agents)
- [Local model runtimes](#local-model-runtimes)
- [Choosing one](#choosing-one)
- [Running agents locally](#running-agents-locally)
- [Questions](#questions)
- [Related lists](#related-lists)

## Personal assistants and autonomous agents

Agents that run as a long-lived process on your machine and talk to you through a terminal,
Telegram, Discord, WhatsApp, Slack or a web page. They remember, schedule, browse and act.

- [OpenClaw](https://github.com/openclaw/openclaw) - A personal AI agent that runs on any OS and talks to you on any platform. The most-starred self-hosted agent on GitHub. Formerly Clawdbot and Moltbot; older guides still use those names and the `~/.clawdbot` or `~/.moltbot` paths.
- [Hermes Agent](https://github.com/NousResearch/hermes-agent) - A self-improving agent from Nous Research with a built-in learning loop. Runs as one gateway process behind Telegram, Discord, Slack, WhatsApp, Signal and a terminal UI, with any model provider or your own endpoint.
- [ZeroClaw](https://github.com/zeroclaw-labs/zeroclaw) - Fast, small, fully autonomous personal assistant infrastructure written in Rust. You own the agent, the data and the machine it runs on.
- [nanoclaw](https://github.com/nanocoai/nanoclaw) - A lightweight OpenClaw alternative that runs each agent in a container for isolation. Connects to WhatsApp, Telegram and Slack.
- [nanobot](https://github.com/HKUDS/nanobot) - A lightweight open source personal agent in Python.
- [Agent Zero](https://github.com/agent0ai/agent-zero) - A general-purpose agent framework that runs in Docker, writes and executes its own code, and can spawn subordinate agents.
- [OpenManus](https://github.com/FoundationAgents/OpenManus) - An open implementation of a general computer-using agent, from the MetaGPT team.
- [agenticSeek](https://github.com/Fosowl/agenticSeek) - A fully local Manus-style agent that thinks, browses and codes with no API keys and no monthly bill.
- [AutoGPT](https://github.com/Significant-Gravitas/AutoGPT) - The original autonomous agent project, now a self-hostable platform for building and running continuous agents.
- [Octop](https://github.com/TencentCloud/Octop) - A self-hosted, multi-user, multi-agent AI assistant.
- [Khoj](https://github.com/khoj-ai/khoj) - A self-hostable AI second brain. Answers from your documents and the web, custom agents, scheduled automations.
- [Leon](https://github.com/leon-ai/leon) - A long-running open source personal assistant with a skills system.
- [PraisonAI](https://github.com/MervinPraison/PraisonAI) - Multi-agent framework and runtime for self-hosted, low-code agent workforces.
- [Kortix](https://github.com/kortix-ai/suna) - Previously Suna. An open source operating system for a company run by multiplayer AI agents.
- [Paperclip](https://github.com/paperclipai/paperclip) - An open source app for managing a workforce of agents.
- [DeerFlow](https://github.com/bytedance/deer-flow) - A long-horizon super-agent harness from ByteDance that researches, codes and creates.
- [Multica](https://github.com/multica-ai/multica) - A self-hostable workspace where humans and AI agents work as one team.
- [IntentKit](https://github.com/crestalnetwork/intentkit) - A self-hosted agent cluster that manages a collaborative team of agents.
- [Huginn](https://github.com/huginn/huginn) - The original self-hosted agent platform: agents that watch the web and act on your behalf, pre-dating LLMs and still maintained.

## Coding agents

Agents that read, write and run code in your repositories. All of these can point at a local
or self-hosted model.

- [OpenHands](https://github.com/OpenHands/OpenHands) - An AI-driven development platform that runs in Docker and works on real repositories.
- [opencode](https://github.com/anomalyco/opencode) - An open source coding agent for the terminal.
- [Cline](https://github.com/cline/cline) - An autonomous coding agent as an SDK, editor extension or CLI.
- [Continue](https://github.com/continuedev/continue) - An open source coding agent and editor assistant with configurable model providers.
- [goose](https://github.com/aaif-goose/goose) - An extensible agent in Rust that installs, runs, edits and tests code, not just suggests it.
- [Open Interpreter](https://github.com/openinterpreter/openinterpreter) - A coding agent built for open models.
- [aider](https://github.com/Aider-AI/aider) - AI pair programming in the terminal, with local model support.
- [SWE-agent](https://github.com/SWE-agent/SWE-agent) - Takes a GitHub issue and tries to fix it with the model of your choice.

## Research agents

- [GPT Researcher](https://github.com/assafelovic/gpt-researcher) - An autonomous agent that performs deep research over the web or your own data with any LLM provider.

DeerFlow, listed above under assistants, is also a long-horizon research harness.

## Browser agents

- [Browser Use](https://github.com/browser-use/browser-use) - A Python library for agents that drive a real browser.
- [Skyvern](https://github.com/Skyvern-AI/skyvern) - Automates browser-based workflows with vision and LLMs. Self-hostable with Docker.
- [Steel](https://github.com/steel-dev/steel-browser) - An open source browser API and sandbox for agents.

## Visual builders and workflow platforms

Low-code tools for building agents and automations in a browser, all installable with Docker.

- [n8n](https://github.com/n8n-io/n8n) - Fair-code workflow automation with native AI agent nodes. The most common self-hosted automation backbone.
- [Dify](https://github.com/langgenius/dify) - A workspace for agentic workflows, RAG pipelines and model management.
- [Langflow](https://github.com/langflow-ai/langflow) - A visual builder for agents and workflows.
- [Activepieces](https://github.com/activepieces/activepieces) - Workflow automation with AI agents and a large MCP server catalogue.
- [Sim](https://github.com/simstudioai/sim) - A collaborative workspace to build, deploy and monitor agents and workflows.
- [Botpress](https://github.com/botpress/botpress) - A hub for building and deploying LLM agents.
- [Obot](https://github.com/obot-platform/obot) - An agent and MCP governance platform.

## Chat interfaces with agents and tools

Self-hosted chat UIs that go past plain chat: tool calling, agents, document search, MCP.

- [Open WebUI](https://github.com/open-webui/open-webui) - A user-friendly interface for Ollama and OpenAI-compatible APIs with tools, functions and pipelines.
- [LibreChat](https://github.com/LibreChat-AI/LibreChat) - An enhanced ChatGPT clone with agents, MCP, skills and every major provider.
- [AnythingLLM](https://github.com/Mintplex-Labs/anything-llm) - A local-first agent and document chat app for desktop or Docker.
- [Jan](https://github.com/janhq/jan) - An open source ChatGPT alternative that runs fully offline on your computer.

## Voice agents

- [Pipecat](https://github.com/pipecat-ai/pipecat) - A framework for voice agents, multimodal apps and realtime AI.
- [LiveKit Agents](https://github.com/livekit/agents) - A framework for realtime voice agents on self-hosted LiveKit.
- [TEN Framework](https://github.com/TEN-framework/ten-framework) - An open source framework for conversational voice agents.
- [Rasa](https://github.com/RasaHQ/rasa) - A machine learning framework for text and voice assistants with dialogue management.

## Agent frameworks

Libraries for writing your own agents. None of these are hosted services; your code runs where you run it.

- [LangGraph](https://github.com/langchain-ai/langgraph) - Build resilient, stateful agents as graphs.
- [LightAgent](https://github.com/wanxingai/LightAgent) - Python framework with tools, memory, MCP, checkpointed workflows, and persistent dynamic task graphs for locally hosted agent applications.
- [CrewAI](https://github.com/crewAIInc/crewAI) - Orchestrate role-playing, collaborating agents.
- [AutoGen](https://github.com/microsoft/autogen) - Microsoft's programming framework for agentic AI.
- [Agno](https://github.com/agno-agi/agno) - A self-driving agent platform and framework.
- [smolagents](https://github.com/huggingface/smolagents) - A barebones library from Hugging Face for agents that think in code.
- [Pydantic AI](https://github.com/pydantic/pydantic-ai) - Typed agents, realtime voice and more for Python, with every model.
- [Semantic Kernel](https://github.com/microsoft/semantic-kernel) - Microsoft's SDK for integrating LLMs into .NET, Python and Java apps.
- [CAMEL](https://github.com/camel-ai/camel) - A multi-agent framework for studying how agents scale.
- [Letta](https://github.com/letta-ai/letta) - A platform for stateful agents with long-term memory that learn over time.

## Memory for agents

- [Mem0](https://github.com/mem0ai/mem0) - A drop-in memory layer for agents and apps, self-hostable.

Letta, listed above under frameworks, is built around long-term memory and can serve as the memory layer on its own.

## Local model runtimes

The engines that serve a model to all of the above without an API key.

- [Ollama](https://github.com/ollama/ollama) - The simplest way to run open models locally, with an OpenAI-compatible API.
- [llama.cpp](https://github.com/ggml-org/llama.cpp) - LLM inference in C and C++ on CPUs and GPUs. Most other runtimes build on it.
- [LocalAI](https://github.com/mudler/LocalAI) - A drop-in OpenAI-compatible server for LLMs, vision, voice and image models on any hardware.
- [vLLM](https://github.com/vllm-project/vllm) - A high-throughput serving engine for LLMs on GPUs.
- [MLC LLM](https://github.com/mlc-ai/mlc-llm) - A universal deployment engine that compiles models for phones, browsers and GPUs.

## Choosing one

| You want                                                         | Start with                                 |
| ---------------------------------------------------------------- | ------------------------------------------ |
| An assistant in Telegram, Discord or WhatsApp that remembers you | OpenClaw, Hermes Agent, ZeroClaw, nanoclaw |
| The same, but every agent sandboxed in a container               | nanoclaw, Agent Zero                       |
| No cloud APIs at all, local models only                          | agenticSeek, Jan, AnythingLLM with Ollama  |
| An agent that works in your code                                 | OpenHands, opencode, goose, Cline          |
| Drag-and-drop automations with AI steps                          | n8n, Dify, Langflow, Activepieces          |
| A chat UI for the whole household or team                        | Open WebUI, LibreChat                      |
| To write your own agent in Python                                | LangGraph, CrewAI, smolagents, Pydantic AI |
| A voice assistant you host                                       | Pipecat, LiveKit Agents, TEN               |

## Running agents locally

Most agents need three things: a model endpoint, a place to run, and somewhere to keep state.

**Model.** Install Ollama or LocalAI from the runtimes section and pull a model. A 7B to 14B model runs on 16 GB of RAM or an 8 GB GPU; 30B and up wants 24 GB of VRAM or a Mac with 32 GB or more. Any agent that accepts an OpenAI-compatible base URL will talk to it.

**Runtime.** Nearly everything here ships a Docker Compose file. A small home server, a NAS with Docker, or a spare mini PC is enough for the agent itself; the model is what needs the memory.

**State.** Agents keep memory, logs and credentials on disk. Put that directory on a volume you back up, and keep the agent on a network you trust, since many of them can run commands and browse.

## Questions

**What is a self-hosted AI agent?** A program that uses a language model to take actions on your behalf, running on hardware you control rather than a vendor's cloud. The model can be local or remote; the agent, its memory and its tools stay with you.

**Can a self-hosted agent run without any cloud API?** Yes. Pair any agent above that accepts an OpenAI-compatible endpoint with Ollama, llama.cpp or LocalAI serving an open model. agenticSeek, Jan and AnythingLLM are built for exactly that.

**What hardware do I need?** The agent itself is light. The model is the cost: 8 GB of VRAM or 16 GB of unified memory runs small models well, and quality climbs with memory. A home server can run the agent while a desktop with a GPU serves the model.

**How is this different from a chatbot?** A chatbot answers. An agent has tools: a shell, a browser, your files, your calendar, other agents. The projects in the first section are the ones that act without being asked each time.

## Related lists

- [awesome-ai-agents](https://github.com/e2b-dev/awesome-ai-agents) - Agents in general, hosted and not.
- [awesome-openclaw-skills](https://github.com/VoltAgent/awesome-openclaw-skills) - Skills for OpenClaw.
- [awesome-hermes-agent](https://github.com/0xNyk/awesome-hermes-agent) - Skills, plugins and memory providers for Hermes Agent.
- [awesome-selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted) - Self-hosted software of every kind.

## Contributing

Additions welcome. A project belongs here if it is open source, can be installed and run on your own machine, and is an agent or something agents are built from or run on. See [contributing.md](contributing.md).
