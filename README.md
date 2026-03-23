<p align="center">
  <picture>
    <img src="https://raw.githubusercontent.com/NousResearch/hermes-agent/main/assets/banner.png" alt="Awesome Hermes Agent" width="600">
  </picture>
</p>

# Awesome Hermes Agent

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of skills, tools, integrations, and resources for enhancing your [Hermes Agent](https://github.com/NousResearch/hermes-agent) workflow — the self-improving AI agent built by [Nous Research](https://nousresearch.com).

Hermes Agent is the only agent with a built-in learning loop — it creates skills from experience, improves them during use, searches its own past conversations, and builds a deepening model of who you are across sessions. Run it on a $5 VPS, a GPU cluster, or serverless infrastructure. Talk to it from Telegram while it works on a cloud VM.

This list tracks the growing ecosystem around it.

---

## Contents

- [Official Resources](#official-resources)
- [Skills & Plugins](#skills--plugins)
  - [Community Skills](#community-skills)
  - [Plugins](#plugins)
  - [agentskills.io Ecosystem](#agentskillsio-ecosystem)
  - [Skill Registries & Discovery](#skill-registries--discovery)
- [Tools & Utilities](#tools--utilities)
  - [Deployment](#deployment)
- [Integrations & Bridges](#integrations--bridges)
- [Multi-Agent & Swarms](#multi-agent--swarms)
- [Domain Applications](#domain-applications)
- [Forks & Derivatives](#forks--derivatives)
- [Guides & Documentation](#guides--documentation)
- [Contributing](#contributing)
- [License](#license)

---

## Official Resources

> Core repositories and resources maintained by Nous Research.

- [Hermes Agent](https://github.com/NousResearch/hermes-agent) by [Nous Research](https://nousresearch.com) - The main event. 10k+ stars and growing. A self-improving AI agent with a closed learning loop, multi-platform gateway (Telegram, Discord, Slack, WhatsApp, Signal), six terminal backends, cron scheduling, and MCP integration. The fact that it migrates from OpenClaw automatically tells you they know their audience.
- [autonovel](https://github.com/NousResearch/autonovel) by [Nous Research](https://nousresearch.com) - Autonomous novel-writing pipeline built on Hermes. If you've ever wanted to ship a 100k-word manuscript without personally writing any of it, this is your pipeline. The output quality is... surprisingly not terrible.
- [hermes-paperclip-adapter](https://github.com/NousResearch/hermes-paperclip-adapter) by [Nous Research](https://nousresearch.com) - Run Hermes as a managed employee in Paperclip companies. If the words "managed employee" in the context of an AI agent don't make you slightly uneasy, you haven't been paying attention. Fascinating integration regardless.
- [hermes-agent-self-evolution](https://github.com/NousResearch/hermes-agent-self-evolution) by [Nous Research](https://nousresearch.com) - Evolutionary self-improvement using DSPy and GEPA (Genetic Evolution of Prompt Architectures). This is the research arm — how Hermes gets better at being Hermes. If you're into meta-learning and agent optimization, start here.
- [Official Documentation](https://hermes-agent.nousresearch.com/docs/) - Comprehensive docs covering quickstart, CLI, configuration, messaging gateway, security, tools, skills, memory, MCP, cron, and architecture. Genuinely well-written.
- [tinker-atropos](https://github.com/NousResearch/tinker-atropos) by [Nous Research](https://nousresearch.com) - Standalone Atropos integration with Thinking Machines Tinker API. The RL training infrastructure that powers Hermes's self-improvement. If you want to fine-tune tool-calling models on real agent trajectories, this is the pipeline.
- [Skills Hub](https://agentskills.io) - The open standard for agent skills. Compatible across Hermes, Claude Code, Cursor, Codex, and other agents. This is where the ecosystem converges.
- [Discord](https://discord.gg/NousResearch) - The Nous Research community. Where bugs get reported, features get requested, and people share things they probably shouldn't.

<br>

## Skills & Plugins

> Skills are procedural memory — reusable capabilities that Hermes creates from experience and improves during use. Plugins extend core functionality.

### Community Skills

- [hermes-plugins](https://github.com/42-evey/hermes-plugins) by [42-evey](https://github.com/42-evey) - Goal management, inter-agent bridge, model selection, and cost control. Four plugins that solve four real problems. The inter-agent bridge alone is worth the install if you're running multiple Hermes instances.
- [hermes-skill-factory](https://github.com/Romanescu11/hermes-skill-factory) by [Romanescu11](https://github.com/Romanescu11) - Meta-skill that auto-generates reusable skills from your workflows. The snake eating its own tail, except useful.
- [litprog-skill](https://github.com/tlehman/litprog-skill) by [tlehman](https://github.com/tlehman) - Literate programming skill that works across Claude Code, OpenCode, and Hermes. If you believe code should read like prose (and you should), this is your skill.
- [Wizards-of-the-Ghosts](https://github.com/Hmbown/Wizards-of-the-Ghosts) by [Hmbown](https://github.com/Hmbown) - Fantasy spell-themed skill pack. Yes, really. Your agent casts "Arcane Refactor" instead of running a linter. It's exactly as fun as it sounds and somehow the skills are actually good.
- [super-hermes](https://github.com/Cranot/super-hermes) by [Cranot](https://github.com/Cranot) - Teaches Hermes to write its own analytical prompts. The beginning of the end, or the beginning of something great. Probably both.
- [hermes-life-os](https://github.com/Lethe044/hermes-life-os) by [Lethe044](https://github.com/Lethe044) - Personal OS agent that detects life patterns and learns about you daily. The most intimate use of Hermes's memory system — it doesn't just remember your code, it remembers your routines. Unsettling and useful in equal measure.
- [hermes-incident-commander](https://github.com/Lethe044/hermes-incident-commander) by [Lethe044](https://github.com/Lethe044) - Autonomous SRE agent for production incident detection and healing. When your server is on fire at 3 AM, this skill wakes up so you don't have to. Pairs beautifully with Hermes's cron scheduling.
- [hermes-agent-skills](https://github.com/zenc-cp/hermes-agent-skills) by [zenc-cp](https://github.com/zenc-cp) - 28 skills for autonomous AI agents. A solid general-purpose skill pack that covers the gaps the built-in skills don't reach.
- [hermes-dojo](https://github.com/Yonkoo11/hermes-dojo) by [Yonkoo11](https://github.com/Yonkoo11) - Self-improvement system that monitors performance, finds weak skills, and fixes them. Like a gym for your agent — except it actually shows up to train.
- [hermes-skill-marketplace](https://github.com/Lethe044/hermes-skill-marketplace) by [Lethe044](https://github.com/Lethe044) - Self-evolving agent that writes, tests, and publishes skills autonomously. The meta-skill to end all meta-skills — your agent builds its own skill economy.
- [traction-skills](https://github.com/farosud/traction-skills) by [farosud](https://github.com/farosud) - 19 growth channel playbooks based on the Traction book. Marketing strategy as agent skills. Your Hermes becomes a growth hacker, for better or worse.

### agentskills.io Ecosystem

> Skills built on the [agentskills.io](https://agentskills.io) open standard — compatible across Hermes and other agent platforms.

- [wondelai/skills](https://github.com/wondelai/skills) by [wondelai](https://github.com/wondelai) - Agent skills for Claude Code and agentskills.io-compatible platforms. A solid cross-platform skills library that works wherever the standard is supported.
- [Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) by [mukul975](https://github.com/mukul975) - 734+ structured cybersecurity skills mapped to MITRE ATT&CK. This is not a toy. If you're doing security work with agents, this is the most comprehensive skills collection available. 3.6k stars for a reason.
- [chainlink-agent-skills](https://github.com/smartcontractkit/chainlink-agent-skills) by [Chainlink](https://github.com/smartcontractkit) - Chainlink agent skills on the agentskills.io spec. When an oracle network publishes agent skills, you know the ecosystem has arrived.
- [black-forest-labs/skills](https://github.com/black-forest-labs/skills) by [Black Forest Labs](https://github.com/black-forest-labs) - FLUX model skills for image generation. The people who made FLUX made these skills. That's really all you need to know.
- [pydantic-ai-skills](https://github.com/DougTrajano/pydantic-ai-skills) by [DougTrajano](https://github.com/DougTrajano) - Pydantic AI with agentskills.io support. Type-safe agent skills. For when you want your agent to fail loudly instead of silently.
- [cognify-skills](https://github.com/Yarmoluk/cognify-skills) by [Yarmoluk](https://github.com/Yarmoluk) - 19 business operations skills. CRM, invoicing, project management — the boring stuff that actually makes money.
- [execplan-skill](https://github.com/tiann/execplan-skill) by [tiann](https://github.com/tiann) - Complex, long-running task execution. When your agent needs to do something that takes more than a few seconds, this skill manages the lifecycle properly.
- [maestro](https://github.com/ReinaMacCredy/maestro) by [ReinaMacCredy](https://github.com/ReinaMacCredy) - Skills with Conductor planning and Beads tracking. An opinionated approach to skill orchestration that actually works in production.
- [bmad-module-skill-forge](https://github.com/armelhbobdad/bmad-module-skill-forge) by [armelhbobdad](https://github.com/armelhbobdad) - Transforms repos and docs into agentskills.io-compliant skills. Feed it a codebase, get skills back. The factory pattern for the skills economy.
- [Agentic-MCP-Skill](https://github.com/cablate/Agentic-MCP-Skill) by [cablate](https://github.com/cablate) - Progressive MCP client with agentskills.io validation. Bridges the MCP protocol world with the skills standard.
- [ripley-xmr-gateway](https://github.com/KYC-rip/ripley-xmr-gateway) by [KYC-rip](https://github.com/KYC-rip) - Monero (XMR) blockchain gateway for agents. Private transactions for your AI. Make of that what you will.
- [skillsdotnet](https://github.com/PederHP/skillsdotnet) by [PederHP](https://github.com/PederHP) - C# implementation of agentskills.io with MCP integration. For the .NET faithful who refuse to write Python.

### Plugins

- [hermes-payguard](https://github.com/nativ3ai/hermes-payguard) by [nativ3ai](https://github.com/nativ3ai) - Safe USDC and x402 payment plugin. Your agent can spend money now. Whether or not this keeps you up at night says a lot about your threat model.
- [hermes-web-search-plus](https://github.com/robbyczgw-cla/hermes-web-search-plus) by [robbyczgw-cla](https://github.com/robbyczgw-cla) - Multi-provider web search with intelligent routing across Serper, Tavily, Exa, and more. The built-in search is fine; this makes it actually good.
- [hermes-weather-plugin](https://github.com/FahrenheitResearch/hermes-weather-plugin) by [FahrenheitResearch](https://github.com/FahrenheitResearch) - NWS-grade model imagery, NEXRAD radar, and meteorological calculations. Not your average weather plugin — this is what actual meteorologists use, packaged for your agent.
- [hermes-wxtrain-plugin](https://github.com/FahrenheitResearch/hermes-wxtrain-plugin) by [FahrenheitResearch](https://github.com/FahrenheitResearch) - ML pipeline plugin for building training datasets from HRRR/GFS/ERA5 weather models. The companion to the weather plugin. Together they form a complete weather research stack inside your agent.
- [hermes-plugin-chrome-profiles](https://github.com/anpicasso/hermes-plugin-chrome-profiles) by [anpicasso](https://github.com/anpicasso) - Switch browser tools between Chrome profiles via CDP. Handy when your agent needs to browse as different identities.
- [hermes-cloudflare](https://github.com/raulvidis/hermes-cloudflare) by [raulvidis](https://github.com/raulvidis) - Cloudflare browser rendering plugin. Headless browsing through Cloudflare's infrastructure — faster and more reliable than local browser automation.
- [evey-bridge-plugin](https://github.com/42-evey/evey-bridge-plugin) by [42-evey](https://github.com/42-evey) - Claude Code plugin for bridging with Evey (hermes-agent). Run Claude Code and Hermes side by side, sharing context. Cross-agent collaboration done right.

### Skill Registries & Discovery

- [hermeshub](https://github.com/amanning3390/hermeshub) by [amanning3390](https://github.com/amanning3390) - Browse, share, and install community skills for Hermes. The emerging community hub for skill discovery. Still young, but the right idea at the right time.
- [skilldock.io](https://github.com/chigwell/skilldock.io) by [chigwell](https://github.com/chigwell) - Registry of reusable AI skills compatible with OpenClaw, Claude Code, and Hermes. A cross-platform skills marketplace that's been around long enough to have real content.

<br>

## Tools & Utilities

> Applications, CLIs, and utilities built on top of or alongside Hermes Agent.

- [hermes-workspace](https://github.com/outsourc-e/hermes-workspace) by [outsourc-e](https://github.com/outsourc-e) - Native web workspace with chat, terminal, memory browser, skills manager, and inspector. Built during the Nous Hackathon 2026 and it shows — this is polished work. If you've been wanting a GUI for Hermes, this is the one.
- [hermes-neurovision](https://github.com/Tranquil-Flow/hermes-neurovision) by [Tranquil-Flow](https://github.com/Tranquil-Flow) - Terminal neurovisualizer with 42 animated themes. Is it necessary? No. Does it make your terminal look like you're hacking the Matrix? Absolutely. Sometimes aesthetics matter.
- [lintlang](https://github.com/roli-lpci/lintlang) by [roli-lpci](https://github.com/roli-lpci) - Static linter for AI agent configs and prompts with HERM v1.1 scoring. Finally, a linter for your agent's personality. Catches the kind of config mistakes that silently degrade your agent's behavior.
- [nix-hermes-agent](https://github.com/0xrsydn/nix-hermes-agent) by [0xrsydn](https://github.com/0xrsydn) - Nix package and NixOS module for Hermes. Reproducible Hermes deployments. If you're a Nix person, you already know why this matters.
- [openclaw-to-hermes](https://github.com/0xNyk/openclaw-to-hermes) by [0xNyk](https://github.com/0xNyk) - Complete migration tool from OpenClaw to Hermes. Battle-tested on real deployments. Handles settings, memories, skills, API keys, messaging configs, and workspace files. If you're still on OpenClaw, this is your escape hatch.
- [vessel-browser](https://github.com/unmodeled-tyler/vessel-browser) by [unmodeled-tyler](https://github.com/unmodeled-tyler) - AI-native Linux browser with MCP control and autonomous browsing. Not a headless browser wrapper — a full browser built from the ground up for agents. Hermes can surf the web like a human, because it has a browser that was designed for exactly that.
- [portable-hermes-agent](https://github.com/rookiemann/portable-hermes-agent) by [rookiemann](https://github.com/rookiemann) - Windows desktop app with 100 tools, GUI, local models, ComfyUI, and workflows. The "I want everything in one package" approach. Surprisingly comprehensive for a portable build.
- [hermes-webui](https://github.com/sanchomuzax/hermes-webui) by [sanchomuzax](https://github.com/sanchomuzax) - Process monitoring and configuration dashboard. A lighter alternative to hermes-workspace — less features, less complexity, more focused on ops.
- [evey-setup](https://github.com/42-evey/evey-setup) by [42-evey](https://github.com/42-evey) - Get the hermes-agent stack running in minutes with free models and 29 plugins. The "just make it work" package. Opinionated defaults, free model access, and a plugin selection that covers most use cases out of the box.
- [flowstate-qmd](https://github.com/amanning3390/flowstate-qmd) by [amanning3390](https://github.com/amanning3390) - Anticipatory memory for AI agents with RAG and vector search. Makes Hermes's memory system even smarter — pre-fetching context before you ask for it.

### Deployment

- [hermes-agent-docker](https://github.com/xmbshwll/hermes-agent-docker) by [xmbshwll](https://github.com/xmbshwll) - Simple Docker sandbox image. The minimal containerized Hermes. Pull, run, done.
- [hermes-agent-template](https://github.com/Crustocean/hermes-agent-template) by [Crustocean](https://github.com/Crustocean) - Generic Docker image for cloud Hermes agents on Crustocean. Production-ready container template with infrastructure wiring pre-configured.
- [portainer-stack-hermes](https://github.com/ellickjohnson/portainer-stack-hermes) by [ellickjohnson](https://github.com/ellickjohnson) - Hermes Agent deployment with ttyd web terminal. Docker Compose + Portainer + web-based terminal access. Deploy Hermes and access it from any browser.
- [hermes-autonomous-server](https://github.com/JackTheGit/hermes-autonomous-server) by [JackTheGit](https://github.com/JackTheGit) - Run Hermes autonomously with systemd and cron on Linux servers. The headless deployment pattern — set it up, walk away, let it work.

<br>

## Integrations & Bridges

> Connect Hermes to other platforms, devices, and services.

- [hermes-android](https://github.com/raulvidis/hermes-android) by [raulvidis](https://github.com/raulvidis) - Android device bridge with a full Python toolset. Control your phone from your agent, or let your agent control your phone. The distinction matters less than you'd think.
- [hermes-miniverse](https://github.com/teknium1/hermes-miniverse) by [teknium1](https://github.com/teknium1) - Bridge to Miniverse pixel worlds. From one of the Nous Research founders — when the people building the agent also build the integrations, things tend to work.
- [zouroboros-swarm-executors](https://github.com/marlandoj/zouroboros-swarm-executors) by [marlandoj](https://github.com/marlandoj) - Local executor bridge for Claude Code + Hermes integration. Run both agents and let them hand off work to each other. The future of multi-agent is interop, and this is a working example.
- [reina](https://github.com/Crustocean/reina) by [Crustocean](https://github.com/Crustocean) - Autonomous AI agent for the Crustocean platform. A purpose-built integration that shows what Hermes looks like when it's deeply embedded in a product.
- [hermes-agent-acp-skill](https://github.com/Rainhoole/hermes-agent-acp-skill) by [Rainhoole](https://github.com/Rainhoole) - Multi-agent delegation skill bridging Hermes, Codex, and Claude Code. The agent dispatcher pattern — Hermes decides which agent is best for each subtask and delegates accordingly.
- [hermes-blockchain-oracle](https://github.com/gizdusum/hermes-blockchain-oracle) by [gizdusum](https://github.com/gizdusum) - Solana blockchain intelligence MCP server. On-chain analytics as an MCP tool — your Hermes can read the blockchain like it reads your filesystem.
- [hermes-council](https://github.com/Ridwannurudeen/hermes-council) by [Ridwannurudeen](https://github.com/Ridwannurudeen) - Adversarial multi-perspective council MCP server. Multiple AI perspectives debate before your agent commits to a decision. Structured disagreement as a feature.
- [NemoHermes](https://github.com/Hmbown/NemoHermes) by [Hmbown](https://github.com/Hmbown) - NVIDIA capability registry and Spark-aware routing layer. Routes compute-heavy tasks to your GPU infrastructure intelligently. If you have NVIDIA hardware, this makes Hermes aware of it.

<br>

## Multi-Agent & Swarms

> Frameworks and tools for running multiple Hermes agents, or Hermes alongside other agents.

- [Ankh.md](https://github.com/Abruptive/Ankh.md) by [Abruptive](https://github.com/Abruptive) - TAW Agent x Hermes multi-agent swarm framework. Named after the Egyptian symbol for life, which is either deeply meaningful or extremely pretentious. The swarm coordination is genuinely impressive either way.
- [gladiator](https://github.com/runtimenoteslabs/gladiator) by [runtimenoteslabs](https://github.com/runtimenoteslabs) - Two zero-human AI companies battle for GitHub stars. A hackathon project that accidentally became a case study in autonomous agent competition. The entertainment value alone is worth the star.
- [bigiron](https://github.com/supermodeltools/bigiron) by [supermodeltools](https://github.com/supermodeltools) - AI-Native SDLC with Hermes and Supermodel code graph. Full software development lifecycle driven by agents. The name "Big Iron" is either a mainframe reference or a Marty Robbins reference, and both are valid.
- [opencode-hermes-multiagent](https://github.com/1ilkhamov/opencode-hermes-multiagent) by [1ilkhamov](https://github.com/1ilkhamov) - 17 specialized agents for OpenCode AI. A well-structured multi-agent system where each agent has a clear role and they communicate through defined interfaces.

<br>

## Domain Applications

> Purpose-built applications using Hermes for specific domains.

- [hermes-embodied](https://github.com/bryercowan/hermes-embodied) by [bryercowan](https://github.com/bryercowan) - Self-improving robotics via VLA model fine-tuning. Built during the Nous Hackathon. The idea of Hermes's learning loop applied to physical robots is either brilliant or terrifying. Probably both.
- [hermescraft](https://github.com/bigph00t/hermescraft) by [bigph00t](https://github.com/bigph00t) - Embodied AI companion for Minecraft with persistent memory. Your agent remembers where you left your diamonds and learns your building style over time. This is the Hermes memory system doing exactly what it was designed to do.
- [Hermes-mars-rover](https://github.com/Snehal707/Hermes-mars-rover) by [Snehal707](https://github.com/Snehal707) - AI-powered Mars rover simulator with ROS2 and Gazebo. Teaching Hermes to navigate another planet. The skill creation loop means the rover literally gets better at roving.
- [anihermes](https://github.com/rodmarkun/anihermes) by [rodmarkun](https://github.com/rodmarkun) - Local anime server and tracker via natural language. "Hey Hermes, what should I watch next?" is now a valid deployment pattern. The recommendation engine is actually decent.
- [job-scout-agent](https://github.com/Christabel337/job-scout-agent) by [Christabel337](https://github.com/Christabel337) - Autonomous job hunting agent. Hermes searches for jobs, tracks applications, and presumably one day will attend the interview for you.
- [hermes-ai-infrastructure-monitoring-toolkit](https://github.com/JackTheGit/hermes-ai-infrastructure-monitoring-toolkit) by [JackTheGit](https://github.com/JackTheGit) - Infrastructure monitoring, cost forecasting, and headless deployment. The DevOps use case for Hermes. Scheduled cron tasks checking your infrastructure and alerting you via Telegram when something's on fire.
- [hermes-genesis](https://github.com/Ridwannurudeen/hermes-genesis) by [Ridwannurudeen](https://github.com/Ridwannurudeen) - Autonomous living world engine with procedural generation. Hermes creates and maintains entire virtual worlds. The skill loop means the worlds get more complex over time. This is either a game engine or a philosophy experiment.
- [hermes-legal](https://github.com/Lethe044/hermes-legal) by [Lethe044](https://github.com/Lethe044) - Autonomous contract risk analysis with English and Turkish support. Feed it a contract, get back the clauses that should worry you. Multi-language legal analysis is a surprisingly natural fit for Hermes's skill system.
- [hermes-startup-architect](https://github.com/dlkakbs/hermes-startup-architect) by [dlkakbs](https://github.com/dlkakbs) - Transforms startup ideas into investor-ready kits — market analysis, pitch deck, financial projections. Whether this replaces a co-founder or a consultant depends on how good the output is. Early reports suggest: pretty good.
- [mercury](https://github.com/hxsteric/mercury) by [hxsteric](https://github.com/hxsteric) - Blockchain cash flow analyzer with multi-chain analysis and WebGL dashboard. On-chain forensics meets beautiful visualization. Name aptly chosen — the messenger god tracking the money god.
- [hermes-research-agent](https://github.com/Aum08Desai/hermes-research-agent) by [Aum08Desai](https://github.com/Aum08Desai) - Research-focused fork for autonomous end-to-end LLM research loops. Literature review, hypothesis generation, experiment design — the full research pipeline in an agent.

<br>

## Forks & Derivatives

> Notable forks and derivative projects that take Hermes in new directions.

- [hermes-agent-camel](https://github.com/nativ3ai/hermes-agent-camel) by [nativ3ai](https://github.com/nativ3ai) - Hermes with integrated CaMeL trust boundaries. Adds formal trust verification to the agent loop. If you need your Hermes to prove it's not doing anything it shouldn't, this is the fork.
- [orahermes-agent](https://github.com/jasperan/orahermes-agent) by [jasperan](https://github.com/jasperan) - Oracle AI Agent Harness — OCI GenAI and Oracle 26ai integration. Hermes wearing an Oracle suit. Enterprise customers, this is your on-ramp.
- [hermes-alpha](https://github.com/kaminocorp/hermes-alpha) by [kaminocorp](https://github.com/kaminocorp) - Cloud-deployed version of Hermes. Pre-configured for cloud deployment with infrastructure templates. Saves you the setup if you just want Hermes running somewhere that isn't your laptop.
- [hermes-skill-distillation](https://github.com/beardthelion/hermes-skill-distillation) by [beardthelion](https://github.com/beardthelion) - Generate agentic training trajectories from real-world tasks. A hackathon project that tackles the hardest problem in agent training — getting high-quality trajectories at scale.

<br>

## Guides & Documentation

> Tutorials, documentation, and learning resources.

- [hermes-agent-docs](https://github.com/mudrii/hermes-agent-docs) by [mudrii](https://github.com/mudrii) - Comprehensive community documentation for Hermes Agent. Covers v0.2.0 in detail. Useful as a supplement to the official docs, especially for deployment patterns.
- [hermes-wsl-ubuntu](https://github.com/metantonio/hermes-wsl-ubuntu) by [metantonio](https://github.com/metantonio) - WSL2 Ubuntu setup instructions. Because "Native Windows is not supported" means someone had to write the WSL guide, and here it is.
- [HermesWiki](https://github.com/martymcenroe/HermesWiki) by [martymcenroe](https://github.com/martymcenroe) - Wiki for building autonomous agents with Hermes. Community-maintained knowledge base with practical patterns and deployment advice.

---

## Contributing

[Recommend a new resource here!](https://github.com/0xNyk/awesome-hermes-agent/issues/new)

Before submitting, please ensure:

1. The resource is directly related to the Hermes Agent ecosystem or the [agentskills.io](https://agentskills.io) standard
2. The resource has a clear README and is reasonably maintained
3. You've checked the list to avoid duplicates

For suggestions about the repository itself, please [open an issue](https://github.com/0xNyk/awesome-hermes-agent/issues/new).

Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting.

## License

[![CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

This list is licensed under [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt this material for any purpose, provided you give appropriate attribution.

All resources included in this list have their own license terms.
