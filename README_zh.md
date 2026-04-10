<p align="center">
  <picture>
    <img src="https://raw.githubusercontent.com/NousResearch/hermes-agent/main/assets/banner.png" alt="Awesome Hermes Agent" width="600">
  </picture>
</p>

# Awesome Hermes Agent

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> 精选的技能、工具、集成和资源列表，用于增强您的 [Hermes Agent](https://github.com/NousResearch/hermes-agent) 工作流——这是由 [Nous Research](https://nousresearch.com) 构建的自我改进型 AI 智能体。

Hermes Agent 是唯一一个内置学习循环的智能体——它从经验中创建技能、在使用中改进、搜索自己的历史对话，并在多个会话中建立对您的深入了解。在 5 美元的 VPS、GPU 集群或无服务器基础设施上运行它。在它于云 VM 上工作时，通过 Telegram 与它对话。

本列表追踪围绕它不断增长的生态系统。

> 生态系统状态（最后审查：2026-04-03）
> - Hermes Agent：[v0.6.0 (v2026.3.30)](https://github.com/NousResearch/hermes-agent/releases/tag/v2026.3.30)
> - 核心仓库：[NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent)（23k+ 星标）
> - 最新发布说明：[Hermes releases](https://github.com/NousResearch/hermes-agent/releases)

---

## 我该从哪里开始？

不熟悉 Hermes？不要试图一次安装所有东西。以下是从零到高效生产的三步路径：

1. **先跑起来** — 按照[官方文档快速入门](https://hermes-agent.nousresearch.com/docs/)操作。它涵盖安装、CLI、配置和您的第一次对话。
2. **添加您的第一个技能** — 安装 [wondelai/skills](https://github.com/wondelai/skills)（380+ 星标，积极维护）——一个跨平台的技能库，适用于 Hermes 和其他智能体。或者尝试 [litprog-skill](https://github.com/tlehman/litprog-skill)（75+ 星标），用于在 Claude Code、OpenCode 和 Hermes 之间进行文学编程。
3. **获取 GUI** — 设置 [hermes-workspace](https://github.com/outsourc-e/hermes-workspace)（500+ 星标），这是一个具有聊天、终端和技能管理器的 Hermes 原生工作区。或者使用 [mission-control](https://github.com/builderz-labs/mission-control)（3.7k+ 星标），这是一个更广泛的智能体编排仪表板，具有车队管理、任务调度和成本跟踪功能。

一旦您适应了，探索下面的完整列表。每个资源都标有成熟度级别，以便您了解将面对什么：

| 标签 | 含义 |
|-----|---------------|
| **production** | 稳定、有文档、积极维护——可以安全地构建 |
| **beta** | 可用但仍在发展——可能会有一些粗糙边缘 |
| **experimental** | 概念验证或早期阶段——可以学习，但不要依赖它 |

---

## 目录

- [我该从哪里开始？](#我该从哪里开始)
- [官方资源](#官方资源)
- [技能与插件](#技能与插件)
  - [社区技能](#社区技能)
  - [插件](#插件)
  - [agentskills.io 生态系统](#agentskillsio-生态系统)
  - [技能注册与发现](#技能注册与发现)
- [工具与实用程序](#工具与实用程序)
  - [部署](#部署)
- [集成与桥接](#集成与桥接)
- [多智能体与蜂群](#多智能体与蜂群)
- [领域应用](#领域应用)
- [分支与衍生项目](#分支与衍生项目)
- [指南与文档](#指南与文档)
- [操作手册](#操作手册)
- [贡献](#贡献)
- [许可证](#许可证)

---

## 官方资源

> 由 Nous Research 维护的核心仓库和资源。

- [Hermes Agent](https://github.com/NousResearch/hermes-agent) by [Nous Research](https://nousresearch.com) - 核心项目。具有闭环学习能力的自我改进型 AI 智能体，多平台网关（Telegram、Discord、Slack、WhatsApp、Signal、飞书/Lark、企业微信）、六个终端后端、cron 调度、MCP 集成、多实例配置文件和备用提供商。23k+ 星标。包括从 OpenClaw 自动迁移。
- [autonovel](https://github.com/NousResearch/autonovel) by [Nous Research](https://nousresearch.com) - 基于 Hermes 构建的自主小说写作流水线。使用智能体循环端到端生成长篇手稿（100k+ 字）。
- [hermes-paperclip-adapter](https://github.com/NousResearch/hermes-paperclip-adapter) by [Nous Research](https://nousresearch.com) - 在 Paperclip 公司中以托管员工身份运行 Hermes。将智能体连接到 Paperclip 的任务管理和治理系统。
- [hermes-agent-self-evolution](https://github.com/NousResearch/hermes-agent-self-evolution) by [Nous Research](https://nousresearch.com) - 使用 DSPy 和 GEPA（遗传进化提示架构）的进化型自我改进。用于优化 Hermes 自身提示和行为的研究流水线。
- [官方文档](https://hermes-agent.nousresearch.com/docs/) - 涵盖快速入门、CLI、配置、消息网关、安全、工具、技能、记忆、MCP、cron、ACP、API 服务器和架构的综合文档。
- [发布说明](https://github.com/NousResearch/hermes-agent/releases) - 官方变更日志，包含每个 Hermes 版本的功能亮点、迁移说明和可靠性修复。
- [tinker-atropos](https://github.com/NousResearch/tinker-atropos) by [Nous Research](https://nousresearch.com) - 与 Thinking Machines Tinker API 的独立 Atropos 集成。用于在真实智能体轨迹上微调工具调用模型的 RL 训练基础设施。
- [技能中心](https://agentskills.io) - 开放的智能体技能开放标准。兼容 Hermes、Claude Code、Cursor、Codex 和其他智能体。
- [Discord](https://discord.gg/NousResearch) - Nous Research 社区。错误报告、功能请求和一般讨论。

<br>

## 技能与插件

> 技能是程序性记忆——Hermes 从经验中创建的可重用能力，并在使用中改进。插件扩展核心功能。

### 社区技能

- **[beta]** [hermes-plugins](https://github.com/42-evey/hermes-plugins) by [42-evey](https://github.com/42-evey) - 目标管理、智能体间桥接、模型选择和成本控制。四个插件覆盖最常见的操作需求。如果您运行多个 Hermes 实例，智能体间桥接很有用。
- **[beta]** [hermes-skill-factory](https://github.com/Romanescu11/hermes-skill-factory) by [Romanescu11](https://github.com/Romanescu11) - 从您的工作流程自动生成可重用技能的元技能。指向您重复的任务，它就会为此创建一个技能。
- **[beta]** [litprog-skill](https://github.com/tlehman/litprog-skill) by [tlehman](https://github.com/tlehman) - 跨 Claude Code、OpenCode 和 Hermes 的文学编程技能。将代码和散文编织成文档化的可执行笔记本。
- **[experimental]** [Wizards-of-the-Ghosts](https://github.com/Hmbown/Wizards-of-the-Ghosts) by [Hmbown](https://github.com/Hmbown) - 奇幻魔法主题技能包。用桌面 RPG 界面包装真实的开发操作（重构、lint、测试）。
- **[experimental]** [super-hermes](https://github.com/Cranot/super-hermes) by [Cranot](https://github.com/Cranot) - 教 Hermes 编写自己的分析提示。添加一个元推理层，智能体在执行任务之前为自己生成更好的提示。
- **[experimental]** [hermes-life-os](https://github.com/Lethe044/hermes-life-os) by [Lethe044](https://github.com/Lethe044) - 检测日常模式并随时间学习您习惯的个人 OS 智能体。使用 Hermes 的记忆系统进行生活方式跟踪，而不仅仅是代码。
- **[beta]** [hermes-incident-commander](https://github.com/Lethe044/hermes-incident-commander) by [Lethe044](https://github.com/Lethe044) - 用于生产事故检测和自我修复的自主 SRE 智能体。监控服务、诊断故障并应用修复。与 Hermes 的 cron 调度配合良好。
- **[beta]** [hermes-dojo](https://github.com/Yonkoo11/hermes-dojo) by [Yonkoo11](https://github.com/Yonkoo11) - 自我改进系统，监控智能体性能、识别薄弱技能并自动迭代。
- **[experimental]** [hermes-skill-marketplace](https://github.com/Lethe044/hermes-skill-marketplace) by [Lethe044](https://github.com/Lethe044) - 自主编写、测试和发布新技能的智能体。自动化技能创建和分发生命周期。


### agentskills.io 生态系统

> 基于 [agentskills.io](https://agentskills.io) 开放标准构建的技能——兼容 Hermes 和其他智能体平台。

- **[production]** [wondelai/skills](https://github.com/wondelai/skills) by [wondelai](https://github.com/wondelai) - 适用于 Claude Code 和 agentskills.io 兼容平台的跨平台智能体技能。
- **[production]** [Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) by [mukul975](https://github.com/mukul975) - 753+ 映射到 MITRE ATT&CK 的结构化网络安全技能。可用的最全面的安全技能集合。4k+ 星标。
- **[production]** [chainlink-agent-skills](https://github.com/smartcontractkit/chainlink-agent-skills) by [Chainlink](https://github.com/smartcontractkit) - agentskills.io 规范上的官方 Chainlink 智能体技能。Oracle 网络数据、CCIP 和智能合约交互。
- **[production]** [black-forest-labs/skills](https://github.com/black-forest-labs/skills) by [Black Forest Labs](https://github.com/black-forest-labs) - FLUX 模型的官方图像生成技能。FLUX 创作者的第一方技能。
- **[production]** [pydantic-ai-skills](https://github.com/DougTrajano/pydantic-ai-skills) by [DougTrajano](https://github.com/DougTrajano) - 支持 agentskills.io 的 Pydantic AI。为智能体技能输入输出添加类型安全的模式验证。
- **[beta]** [cognify-skills](https://github.com/Yarmoluk/cognify-skills) by [Yarmoluk](https://github.com/Yarmoluk) - 涵盖 CRM、开票和项目管理的 19 项业务运营技能。
- **[beta]** [execplan-skill](https://github.com/tiann/execplan-skill) by [tiann](https://github.com/tiann) - 管理复杂长时间运行的任务执行，具有适当的生命周期处理——进度跟踪、检查点和故障恢复。
- **[beta]** [maestro](https://github.com/ReinaMacCredy/maestro) by [ReinaMacCredy](https://github.com/ReinaMacCredy) - 具有 Conductor 规划和 Beads 跟踪的技能编排。将多步骤技能执行构建为可观察的流水线。
- **[beta]** [bmad-module-skill-forge](https://github.com/armelhbobdad/bmad-module-skill-forge) by [armelhbobdad](https://github.com/armelhbobdad) - 将仓库和文档转换为 agentskills.io 合规技能。输入代码库，输出可安装的技能。
- **[beta]** [Agentic-MCP-Skill](https://github.com/cablate/Agentic-MCP-Skill) by [cablate](https://github.com/cablate) - 带 agentskills.io 验证的 MCP 客户端。将 MCP 工具服务器与技能标准桥接。
- **[experimental]** [ripley-xmr-gateway](https://github.com/KYC-rip/ripley-xmr-gateway) by [KYC-rip](https://github.com/KYC-rip) - 用于智能体的 Monero (XMR) 区块链网关。实现从智能体工作流的私人加密货币交易。
- **[beta]** [skillsdotnet](https://github.com/PederHP/skillsdotnet) by [PederHP](https://github.com/PederHP) - agentskills.io 的 C# 实现，带 MCP 集成。Python/TypeScript SDK 的 .NET 替代方案。

### 插件

- **[beta]** [plur](https://github.com/plur-ai/plur) by [plur-ai](https://github.com/plur-ai) - AI 智能体的共享记忆层，采用开放的 engram 格式（YAML）。用于 Hermes 工作流中持久的学习模式。
- **[experimental]** [hermes-payguard](https://github.com/nativ3ai/hermes-payguard) by [nativ3ai](https://github.com/nativ3ai) - 安全的 USDC 和 x402 支付插件。让 Hermes 发送和接收具有可配置消费限制和审批流程的支付。
- **[beta]** [hermes-web-search-plus](https://github.com/robbyczgw-cla/hermes-web-search-plus) by [robbyczgw-cla](https://github.com/robbyczgw-cla) - 跨 Serper、Tavily、Exa 等的智能路由多提供商网络搜索。用更好的结果质量和来源多样性替换内置搜索。
- **[beta]** [hermes-weather-plugin](https://github.com/FahrenheitResearch/hermes-weather-plugin) by [FahrenheitResearch](https://github.com/FahrenheitResearch) - 专业级天气插件，具有 NWS 模型图像、NEXRAD 雷达和气象计算。
- **[experimental]** [hermes-wxtrain-plugin](https://github.com/FahrenheitResearch/hermes-wxtrain-plugin) by [FahrenheitResearch](https://github.com/FahrenheitResearch) - 从 HRRR/GFS/ERA5 天气模型构建训练数据集的 ML 流水线插件。构建天气 ML 流水线的天气插件配套工具。
- **[experimental]** [hermes-plugin-chrome-profiles](https://github.com/anpicasso/hermes-plugin-chrome-profiles) by [anpicasso](https://github.com/anpicasso) - 通过 CDP 在 Chrome 配置文件之间切换浏览器工具。用于多账户测试或使用不同保存会话进行浏览。
- **[experimental]** [hermes-cloudflare](https://github.com/raulvidis/hermes-cloudflare) by [raulvidis](https://github.com/raulvidis) - Cloudflare 浏览器渲染插件。通过 Cloudflare 基础设施进行无头浏览，而不是本地浏览器自动化。
- **[beta]** [evey-bridge-plugin](https://github.com/42-evey/evey-bridge-plugin) by [42-evey](https://github.com/42-evey) - 与 Evey (hermes-agent) 桥接的 Claude Code 插件。让 Claude Code 和 Hermes 共享上下文并在彼此之间交接任务。

### 技能注册与发现

- **[beta]** [hermeshub](https://github.com/amanning3390/hermeshub) by [amanning3390](https://github.com/amanning3390) - 浏览、分享和安装 Hermes 社区技能。技能发现的社区中心，仍处于早期但正在增长。
- **[production]** [skilldock.io](https://github.com/chigwell/skilldock.io) by [chigwell](https://github.com/chigwell) - 兼容 OpenClaw、Claude Code 和 Hermes 的可重用 AI 技能注册表成熟的跨平台技能市场，有活跃的目录。

<br>

## 工具与实用程序

> 构建在 Hermes Agent 之上或旁边的应用程序、CLI 和实用程序。

- **[production]** [hermes-workspace](https://github.com/outsourc-e/hermes-workspace) by [outsourc-e](https://github.com/outsourc-e) - 具有聊天、终端、记忆浏览器、技能管理器和检查器的基于 Web 的工作区。适用于 Hermes 的最完整 GUI。在 Nous Hackathon 2026 期间构建。
- **[production]** [mission-control](https://github.com/builderz-labs/mission-control) by [builderz-labs](https://github.com/builderz-labs) - AI 智能体编排的开源仪表板。管理智能体车队、调度任务、跟踪成本和协调多智能体工作流。自托管，SQLite 驱动。3.7k+ 星标。
- **[experimental]** [hermes-neurovision](https://github.com/Tranquil-Flow/hermes-neurovision) by [Tranquil-Flow](https://github.com/Tranquil-Flow) - 具有 42 个动画主题的终端神经可视化器。智能体活动的装饰终端覆盖。
- **[beta]** [lintlang](https://github.com/roli-lpci/lintlang) by [roli-lpci](https://github.com/roli-lpci) - 带 HERM v1.1 评分的 AI 智能体配置和提示的静态 lint 工具。捕获会静默降低智能体行为的配置错误。
- **[beta]** [nix-hermes-agent](https://github.com/0xrsydn/nix-hermes-agent) by [0xrsydn](https://github.com/0xrsydn) - Hermes 的 Nix 包和 NixOS 模块。通过 Nix flakes 实现完全可复现的部署。
- **[beta]** [openclaw-to-hermes](https://github.com/0xNyk/openclaw-to-hermes) by [0xNyk](https://github.com/0xNyk) - 从 OpenClaw 到 Hermes 的社区迁移工具。在原生 `hermes-migrate` 有关键错误时构建。对于 Hermes v0.3.0+，首选原生 `hermes claw migrate` 命令——它现在覆盖完整的迁移路径。
- **[experimental]** [vessel-browser](https://github.com/unmodeled-tyler/vessel-browser) by [unmodeled-tyler](https://github.com/unmodeled-tyler) - 具有 MCP 控制和自主浏览的 AI 原生 Linux 浏览器。为智能体使用而构建的完整浏览器，而非无头包装器。
- **[beta]** [portable-hermes-agent](https://github.com/rookiemann/portable-hermes-agent) by [rookiemann](https://github.com/rookiemann) - Windows 桌面应用，在单个便携式包中捆绑 100 个工具、GUI、本地模型、ComfyUI 和工作流。
- **[beta]** [hermes-webui](https://github.com/sanchomuzax/hermes-webui) by [sanchomuzax](https://github.com/sanchomuzax) - 轻量级进程监控和配置仪表板。作为 hermes-workspace 的更简单替代方案，专注于运维。
- **[beta]** [evey-setup](https://github.com/42-evey/evey-setup) by [42-evey](https://github.com/42-evey) - 一键设置完整的 hermes-agent 堆栈，包含免费模型和 29 个插件。涵盖大多数用例的固执默认配置。
- **[beta]** [flowstate-qmd](https://github.com/amanning3390/flowstate-qmd) by [amanning3390](https://github.com/amanning3390) - 具有 RAG 和向量搜索的 AI 智能体预期记忆。在查询到达智能体之前预取相关上下文。

### 部署

- **[beta]** [hermes-agent-docker](https://github.com/xmbshwll/hermes-agent-docker) by [xmbshwll](https://github.com/xmbshwll) - Hermes 的最小 Docker 沙箱镜像。拉取、运行、完成。
- **[beta]** [hermes-agent-template](https://github.com/Crustocean/hermes-agent-template) by [Crustocean](https://github.com/Crustocean) - 用于在 Crustocean 上云端 Hermes 部署的生产就绪 Docker 镜像。基础设施布线预配置。
- **[experimental]** [portainer-stack-hermes](https://github.com/ellickjohnson/portainer-stack-hermes) by [ellickjohnson](https://github.com/ellickjohnson) - Docker Compose + Portainer + ttyd Web 终端。部署 Hermes 并从任何浏览器访问它。
- **[experimental]** [hermes-autonomous-server](https://github.com/JackTheGit/hermes-autonomous-server) by [JackTheGit](https://github.com/JackTheGit) - 在 Linux 服务器上使用 systemd 和 cron 的无人值守 Hermes 部署。无人值守运行。

<br>

## 集成与桥接

> 将 Hermes 连接到其他平台、设备和服务。

- **[beta]** [hermes-android](https://github.com/raulvidis/hermes-android) by [raulvidis](https://github.com/raulvidis) - 具有完整 Python 工具集的 Android 设备桥接。让 Hermes 与 Android 设备交互和控制。
- **[beta]** [hermes-miniverse](https://github.com/teknium1/hermes-miniverse) by [teknium1](https://github.com/teknium1) - 通往 Miniverse 像素世界的桥接。由 Nous Research 联合创始人创建。
- **[production]** [hindsight](https://github.com/vectorize-io/hindsight) by [Vectorize](https://github.com/vectorize-io) - 具有 retain/recall/reflect 工作流的智能体长期记忆层。通过插件或 MCP 与 Hermes 集成，支持语义、图谱和时间检索。
- **[beta]** [honcho-self-hosted](https://github.com/elkimek/honcho-self-hosted) by [elkimek](https://github.com/elkimek) - Hermes 的自托管 Honcho 记忆后端设置。当您需要更强的跨会话记忆行为和本地控制时很有用。
- **[experimental]** [zouroboros-swarm-executors](https://github.com/marlandoj/zouroboros-swarm-executors) by [marlandoj](https://github.com/marlandoj) - Claude Code + Hermes 集成的本地执行器桥接。实现两个智能体之间的任务交接。
- **[beta]** [reina](https://github.com/Crustocean/reina) by [Crustocean](https://github.com/Crustocean) - Crustocean 平台的自主 AI 智能体。Hermes 与 Crustocean 产品的深度集成。
- **[beta]** [hermes-agent-acp-skill](https://github.com/Rainhoole/hermes-agent-acp-skill) by [Rainhoole](https://github.com/Rainhoole) - 桥接 Hermes、Codex 和 Claude Code 的多智能体委托技能。自动将子任务路由到最合适的智能体。
- **[experimental]** [hermes-blockchain-oracle](https://github.com/gizdusum/hermes-blockchain-oracle) by [gizdusum](https://github.com/gizdusum) - Solana 区块链智能 MCP 服务器。通过 MCP 向 Hermes 提供链上分析和钱包数据。
- **[experimental]** [hermes-council](https://github.com/Ridwannurudeen/hermes-council) by [Ridwannurudeen](https://github.com/Ridwannurudeen) - 对抗性多视角委员会 MCP 服务器。多个 AI 视角在智能体承诺决策之前进行辩论。
- **[experimental]** [NemoHermes](https://github.com/Hmbown/NemoHermes) by [Hmbown](https://github.com/Hmbown) - NVIDIA 能力注册表和 Spark 感知路由层。将计算密集型任务路由到可用的 GPU 基础设施。

<br>

## 多智能体与蜂群

> 用于运行多个 Hermes 智能体或 Hermes 与其他智能体一起运行的框架和工具。

- **[experimental]** [Ankh.md](https://github.com/Abruptive/Ankh.md) by [Abruptive](https://github.com/Abruptive) - TAW Agent x Hermes 多智能体蜂群框架。协调多个具有共同目标和分布式任务执行的智能体。
- **[experimental]** [gladiator](https://github.com/runtimenoteslabs/gladiator) by [runtimenoteslabs](https://github.com/runtimenoteslabs) - 两个自主 AI 公司争夺 GitHub 星标。探索自主智能体竞争动态的黑客马拉松项目。
- **[beta]** [bigiron](https://github.com/supermodeltools/bigiron) by [supermodeltools](https://github.com/supermodeltools) - 具有 Hermes 和 Supermodel 代码图的 AI 原生 SDLC。由协调的智能体驱动的完整软件开发生命周期。
- **[beta]** [opencode-hermes-multiagent](https://github.com/1ilkhamov/opencode-hermes-multiagent) by [1ilkhamov](https://github.com/1ilkhamov) - 适用于 OpenCode AI 的 17 个专业智能体。每个智能体都有定义的角色，它们通过结构化接口进行通信。

<br>

## 领域应用

> 使用 Hermes 针对特定领域构建的专用应用程序。

- **[experimental]** [hermes-embodied](https://github.com/bryercowan/hermes-embodied) by [bryercowan](https://github.com/bryercowan) - 通过 VLA 模型微调的自我改进机器人。将 Hermes 学习循环应用于物理机器人控制。Nous Hackathon 项目。
- **[beta]** [hermescraft](https://github.com/bigph00t/hermescraft) by [bigph00t](https://github.com/bigph00t) - 具有持久记忆的 Minecraft 具身 AI 伴侣。跟踪库存、学习建筑偏好并在会话中保留上下文。
- **[experimental]** [Hermes-mars-rover](https://github.com/Snehal707/Hermes-mars-rover) by [Snehal707](https://github.com/Snehal707) - 具有 ROS2 和 Gazebo 的火星探测器模拟器。使用 Hermes 的技能创建循环随时间改进导航。
- **[beta]** [anihermes](https://github.com/rodmarkun/anihermes) by [rodmarkun](https://github.com/rodmarkun) - 具有自然语言界面的本地动漫服务器和跟踪器。通过对话浏览、跟踪和获取推荐。
- **[beta]** [job-scout-agent](https://github.com/Christabel337/job-scout-agent) by [Christabel337](https://github.com/Christabel337) - 自主求职智能体。搜索列表、跟踪申请并管理求职流水线。
- **[beta]** [hermes-ai-infrastructure-monitoring-toolkit](https://github.com/JackTheGit/hermes-ai-infrastructure-monitoring-toolkit) by [JackTheGit](https://github.com/JackTheGit) - 通过 Telegram 进行基础设施监控、成本预测和警报。使用 cron 调度进行持续检查。
- **[experimental]** [hermes-genesis](https://github.com/Ridwannurudeen/hermes-genesis) by [Ridwannurudeen](https://github.com/Ridwannurudeen) - 具有程序生成的自主生活世界引擎。创建并维护随时间复杂度增加而增长的虚拟世界。
- **[experimental]** [hermes-legal](https://github.com/Lethe044/hermes-legal) by [Lethe044](https://github.com/Lethe044) - 具有英语和土耳其语支持的合同风险分析。识别风险条款并总结法律义务。
- **[beta]** [hermes-startup-architect](https://github.com/dlkakbs/hermes-startup-architect) by [dlkakbs](https://github.com/dlkakbs) - 从创业想法生成投资就绪的工具包——市场分析、推介甲板和财务预测。
- **[beta]** [mercury](https://github.com/hxsteric/mercury) by [hxsteric](https://github.com/hxsteric) - 带 WebGL 仪表板的多链区块链现金流分析器。链上取证和流可视化。
- **[experimental]** [hermes-research-agent](https://github.com/Aum08Desai/hermes-research-agent) by [Aum08Desai](https://github.com/Aum08Desai) - 自主 LLM 研究智能体。端到端处理文献综述、假设生成和实验设计。

<br>

## 分支与衍生项目

> 将 Hermes 推向新方向的重要分支和衍生项目。

- **[beta]** [hermes-agent-camel](https://github.com/nativ3ai/hermes-agent-camel) by [nativ3ai](https://github.com/nativ3ai) - 集成 CaMeL 信任边界线的 Hermes。为安全关键部署添加形式化信任验证到智能体循环。
- **[experimental]** [orahermes-agent](https://github.com/jasperan/orahermes-agent) by [jasperan](https://github.com/jasperan) - Oracle AI 智能体工具——OCI GenAI 和 Oracle 26ai 集成。Oracle 环境的企业入口。
- **[beta]** [hermes-alpha](https://github.com/kaminocorp/hermes-alpha) by [kaminocorp](https://github.com/kaminocorp) - 具有预配置基础设施模板的云部署 Hermes。跳过本地设置。
- **[experimental]** [hermes-skill-distillation](https://github.com/beardthelion/hermes-skill-distillation) by [beardthelion](https://github.com/beardthelion) - 从现实世界任务生成智能体训练轨迹。用于大规模生成微调数据的黑客马拉松项目。

<br>

## 指南与文档

> 教程、文档和学习资源。

- **[beta]** [hermes-agent-docs](https://github.com/mudrii/hermes-agent-docs) by [mudrii](https://github.com/mudrii) - Hermes Agent 的综合社区文档。详细涵盖 v0.2.0，是部署模式的官方文档的有用补充。
- **[production]** [hermes-wsl-ubuntu](https://github.com/metantonio/hermes-wsl-ubuntu) by [metantonio](https://github.com/metantonio) - 在 Windows 上运行 Hermes 的分步 WSL2 Ubuntu 设置说明。
- **[beta]** [HermesWiki](https://github.com/martymcenroe/HermesWiki) by [martymcenroe](https://github.com/martymcenroe) - 社区维护的维基，包含使用 Hermes 构建自主智能体的实用模式和部署建议。

---

## 操作手册

> 在生产中反复帮助 Hermes 团队的实用工作流模式。

- **夜间自我进化 + 护栏评估** — 按计划运行 [hermes-agent-self-evolution](https://github.com/NousResearch/hermes-agent-self-evolution)，然后运行第二个验证 cron 来评分质量并阻止优化循环游戏。
- **使用 Honcho/Hindsight 处理记忆压力** — 如果您重复上下文或丢失长期回忆，请查看 [Honcho Memory 文档](https://hermes-agent.nousresearch.com/docs/user-guide/features/honcho)，并评估 [hindsight](https://github.com/vectorize-io/hindsight) 或自托管记忆后端。
- **尽早调整会话超时/过期** — 使用[配置文档](https://hermes-agent.nousresearch.com/docs/user-guide/configuration/)调整较慢线程的会话保留，以便在需要时保持上下文。
- **OpenClaw 并行迁移** — 在迁移期间使用 [openclaw-to-hermes](https://github.com/0xNyk/openclaw-to-hermes) 和原生 Hermes 迁移路径保持两个系统运行，然后在 cron 和路由行为匹配后切换。
- **有意识地策展 USER.md 和 MEMORY.md** — 将配置文件记忆视为高信号基础设施。保持条目简洁、持久和偏好导向，而不是倾倒原始笔记。

---

## 贡献

[在此推荐新资源！](https://github.com/0xNyk/awesome-hermes-agent/issues/new)

提交前，请确保：

1. 该资源与 Hermes Agent 生态系统或 [agentskills.io](https://agentskills.io) 标准直接相关
2. 该资源有清晰的 README 并被合理维护
3. 您已检查列表以避免重复

关于仓库本身的建议，请[提交问题](https://github.com/0xNyk/awesome-hermes-agent/issues/new)。

提交前请阅读 [CONTRIBUTING.md](CONTRIBUTING.md)。


---

<div align="center">

**需要为您的团队构建智能体基础设施、交易系统或 Solana 应用程序吗？**

[Builderz](https://builderz.dev) 交付生产级 AI 系统——15 个国家的 32+ 产品。

[联系我们](https://builderz.dev) | [@nyk_builderz](https://x.com/nyk_builderz)

</div>

## 许可证

[![CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

本列表采用[知识共享署名 4.0 国际许可](https://creativecommons.org/licenses/by/4.0/)。您可以自由共享和改编此材料供任何目的使用，但须提供适当的归属。

本列表中包含的所有资源均有其自己的许可条款。
