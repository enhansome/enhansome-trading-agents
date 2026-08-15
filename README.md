# Awesome trading agents with stars

<!--lint disable awesome-heading double-link-->

<div align="center">

<img src="assets/header-generated-v2.png" alt="Awesome Trading Agents — The Trading Agentic Stack" width="760" />

<p><strong>English</strong> · <a href="README.zh-CN.md">简体中文</a></p>

<p>
  <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome" /></a>
  <a href="https://github.com/LLMQuant/awesome-trading-agents"><img src="https://img.shields.io/github/stars/LLMQuant/awesome-trading-agents?style=flat" alt="GitHub stars" /></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-CC0%201.0-lightgrey.svg" alt="License: CC0-1.0" /></a>
  <a href="https://github.com/topics/trading-agents"><img src="https://img.shields.io/badge/topics-trading--agents%20%C2%B7%20mcp--servers%20%C2%B7%20agent--skills-blue" alt="Topics" /></a>
  <a href="https://github.com/LLMQuant/awesome-trading-agents/commits"><img src="https://img.shields.io/github/last-commit/LLMQuant/awesome-trading-agents" alt="Last commit" /></a>
  <a href="README.zh-CN.md"><img src="https://img.shields.io/badge/bilingual-zh%20%C2%B7%20en-708090" alt="Bilingual" /></a>
</p>

</div>

Awesome Trading Agents collects open-source projects where LLMs help research markets, make trading decisions, or connect agents to market data and execution tools. The list focuses on three building blocks: Agents, MCPs, and Skills. It does not try to cover classic quant libraries, time-series models, or reinforcement-learning trading bots; those are better served by [`georgezouq/awesome-ai-in-finance`](https://github.com/georgezouq/awesome-ai-in-finance) ⭐ 6,400 | 🐛 30 | 📅 2026-08-04 and [`wilsonfreitas/awesome-quant`](https://github.com/wilsonfreitas/awesome-quant) ⭐ 28,772 | 🐛 59 | 🌐 HTML | 📅 2026-08-15. Entries are selected for public code or artifacts, clear LLM-driven behavior, recent activity, useful documentation, a distinct role, and visible adoption. Stewarded by the [LLMQuant](https://llmquant.com) community.

> \[!TIP]
> **If you only read three:**
>
> * **Agents** — [TauricResearch/TradingAgents](#agents-tradingagents) · [virattt/ai-hedge-fund](#agents-ai-hedge-fund) · [HKUDS/AI-Trader](#agents-ai-trader)
> * **MCPs** — [alpacahq/alpaca-mcp-server](#mcps-alpaca) · [krakenfx/kraken-cli](#mcps-kraken-cli) · [financial-datasets/mcp-server](#mcps-financial-datasets)
> * **Skills** — [tradermonty/claude-trading-skills](#skills-claude-trading-skills) · [himself65/finance-skills](#skills-finance-skills) · [RKiding/Awesome-finance-skills](#skills-alphaear)

> \[!NOTE]
> Dates are not shown after every item. We still check recent activity before adding or updating a project; the README only keeps details that help readers choose a project, such as official status, forks, or useful pairings.

<!--lint disable awesome-toc-->

## Contents

* [**Agents**](#agents)
  * [Multi-agent trading systems](#agents-multi-agent)
  * [Single-agent end-to-end traders](#agents-single-agent)
  * [Research / equity-research copilots](#agents-research-copilots)
  * [Real-money / competition experiments](#agents-real-money)
  * [Prediction-market specialists](#agents-prediction-market)
  * [Benchmarks & evaluations](#agents-benchmarks)
  * [Strategy coding / self-improving agents](#agents-strategy-coding)
* [**MCPs**](#mcps)
  * [Market data / data providers](#mcps-market-data)
  * [Brokerage / exchange trading](#mcps-brokerage)
  * [Research tools / analysis](#mcps-research-tools)
  * [TradingView bridge](#mcps-tradingview)
  * [Prediction markets](#mcps-prediction-market)
  * [Strategy / backtesting platforms](#mcps-backtesting)
* [**Skills**](#skills)
  * [Equity research](#skills-equity-research)
  * [Crypto / DeFi / on-chain](#skills-crypto)
  * [Strategy coding & backtesting](#skills-strategy-coding)
  * [Brokerage execution & portfolio](#skills-brokerage)
* [**Resources**](#resources)
  * [Papers](#resources-papers)
  * [Learn](#resources-learn)
* [Related awesome lists](#related-awesome-lists)

<!--lint enable awesome-toc-->

<a id="agents"></a>

## Agents

<p align="center">
  <img src="assets/section-agents.png" alt="Agents section header" width="760" />
</p>

Agents are projects where an LLM is part of the actual research or trading decision. This includes analyst teams, single-agent traders, research copilots, live trading experiments, benchmarks, and tools that write or improve strategies. The TradingAgents forks are listed at the same level as the original project so the section stays easy to scan.

<a id="agents-multi-agent"></a>

### Multi-agent trading systems

<a id="agents-tradingagents"></a>

* [TauricResearch/TradingAgents](https://github.com/TauricResearch/TradingAgents) ⭐ 98,204 | 🐛 362 | 🌐 Python | 📅 2026-07-18 - Multi-agent trading framework where analysts, bull/bear researchers, a trader, risk control, and a portfolio manager debate before making a decision; built with LangGraph.
* [hsliuping/TradingAgents-CN](https://github.com/hsliuping/TradingAgents-CN) ⭐ 31,139 | 🐛 286 | 🌐 Python | 📅 2026-07-24 - Chinese-localised TradingAgents fork tuned for A-shares; Tushare / AkShare data sources + Chinese-language reports + A-share regulatory context. *(← fork of TauricResearch/TradingAgents.)*
* [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) ⭐ 30,870 | 🐛 16 | 🌐 Python | 📅 2026-08-14 - Personal multi-agent finance workspace from HKUDS Lab; bundles Skills, MCP tools, and swarm presets across A-shares, HK, US, crypto, futures, and forex.
* [HKUDS/AI-Trader](https://github.com/HKUDS/AI-Trader) ⭐ 21,411 | 🐛 43 | 🌐 Python | 📅 2026-06-11 - "Agent-native trading platform"; any AI agent (OpenClaw / nanobot / Claude Code / Codex / Cursor) registers via SKILL.md and trades live on AI4trade.ai; multi-asset + copy-trading + cross-platform sync.
* [ValueCell-ai/valuecell](https://github.com/ValueCell-ai/valuecell) ⭐ 10,997 | 🐛 66 | 🌐 Python | 📅 2026-03-09 - Community finance workspace with research, strategy, and news agents; connects to Binance, OKX, and Hyperliquid; includes macOS and Windows desktop apps.
* [brokermr810/QuantDinger](https://github.com/brokermr810/QuantDinger) ⭐ 10,682 | 🐛 54 | 🌐 Python | 📅 2026-08-14 - Open-source AI quant-trading platform; combines multi-agent research, backtesting, live trading, and multi-exchange routing.
* [AI4Finance-Foundation/FinRobot](https://github.com/AI4Finance-Foundation/FinRobot) ⭐ 7,784 | 🐛 72 | 🌐 Jupyter Notebook | 📅 2026-07-27 - AI4Finance Foundation's open-source finance AI agent platform; useful for academic-style stock research, market forecasting, and report generation. <a id="agents-vibe-trading"></a>
* [The-Swarm-Corporation/AutoHedge](https://github.com/The-Swarm-Corporation/AutoHedge) ⭐ 4,173 | 🐛 17 | 🌐 Python | 📅 2026-05-11 - "Spin up an autonomous hedge fund in minutes"; applies the Swarms framework to market analysis, risk, and execution; CLI / SDK first.
* [olaxbt/ai-market-maker](https://github.com/olaxbt/ai-market-maker) ⭐ 2,105 | 🐛 1 | 🌐 Python | 📅 2026-08-14 - Agentic crypto hedge-fund stack with specialist agents, Risk Guard, backtests, paper trading, and OpenClaw packaging. <a id="agents-langalpha"></a>
* [Lumiwealth/lumibot](https://github.com/Lumiwealth/lumibot) ⭐ 1,927 | 🐛 88 | 🌐 Python | 📅 2026-08-13 - Backtestable AI trading-agent/team runtime with research, debate, risk, and memory in one backtest/paper/live strategy loop.
* [oficcejo/aiagents-stock](https://github.com/oficcejo/aiagents-stock) ⭐ 1,843 | 🐛 24 | 🌐 Python | 📅 2026-07-27 - A-share multi-agent analyst team with dragon-and-tiger list tracking, sector-rotation alerts, and a miniqmt execution hook. *(← inspired by TradingAgents.)* <a id="agents-ai-trader"></a>
* [ginlix-ai/LangAlpha](https://github.com/ginlix-ai/LangAlpha) ⭐ 1,648 | 🐛 20 | 🌐 Python | 📅 2026-08-15 - "Claude Code for finance"; LangChain + LangGraph multi-agent investment workbench; integrates Agents · MCPs · Skills in one repo.
* [ygwyg/MAHORAGA](https://github.com/ygwyg/MAHORAGA) ⭐ 865 | 🐛 6 | 🌐 TypeScript | 📅 2026-02-17 - TypeScript crypto-trading agent focused on social sentiment analysis and adaptive learning; useful if you want a TypeScript implementation.
* [KylinMountain/TradingAgents-AShare](https://github.com/KylinMountain/TradingAgents-AShare) ⭐ 772 | 🐛 21 | 🌐 Python | 📅 2026-08-14 - A-share rewrite; 15 agents + visual UI + OpenClaw / Claude Code integration + one-click Docker deploy. *(← fork of TauricResearch/TradingAgents.)*
* [dragon1086/prism-insight](https://github.com/dragon1086/prism-insight) ⭐ 721 | 🐛 3 | 🌐 Python | 📅 2026-08-13 - Korean-market-focused multi-agent stock-analysis and trading system; built-in MCP integration.
* [FinStep-AI/ContestTrade](https://github.com/FinStep-AI/ContestTrade) ⭐ 674 | 🐛 16 | 🌐 Python | 📅 2025-12-22 - Multi-agent trading system where agents compete internally before one view is selected for the final decision.
* [51bitquant/ai-hedge-fund-crypto](https://github.com/51bitquant/ai-hedge-fund-crypto) ⭐ 615 | 🐛 12 | 🌐 Python | 📅 2025-09-05 - Crypto-focused fork of virattt/ai-hedge-fund; multi-timeframe analysis + strategy ensemble + crypto market-data access. <a id="agents-prism-insight"></a>
* [EthanAlgoX/LLM-TradeBot](https://github.com/EthanAlgoX/LLM-TradeBot) ⭐ 311 | 🐛 7 | 🌐 TypeScript | 📅 2026-08-08 - Multi-agent crypto-trading system; Binance real-time execution + adaptive strategy switching; combines ideas from TradingAgents and nof1.ai.
* [Tomortec/CryptoTradingAgents](https://github.com/Tomortec/CryptoTradingAgents) ⭐ 274 | 🐛 1 | 🌐 Python | 📅 2025-12-22 - Multi-agent LLM crypto-trading framework; applies the TradingAgents idea to crypto trading.
* [YichengYang-Ethan/oracle3](https://github.com/YichengYang-Ethan/oracle3) ⭐ 256 | 🐛 17 | 🌐 Python | 📅 2026-05-08 - Multi-venue (Kalshi / Polymarket / Solana) prediction-market autonomous agent; Wang-Transform pricing + Kelly criterion + cross-venue arbitrage.
* [huygiatrng/AlpacaTradingAgent](https://github.com/huygiatrng/AlpacaTradingAgent) ⭐ 252 | 🐛 0 | 🌐 Python | 📅 2026-07-18 - TradingAgents-style multi-agent framework connected to Alpaca for US-equity trading. *(→ pairs with: [alpacahq/alpaca-mcp-server](#mcps-alpaca).)*
* [Yaolinwang/AITD](https://github.com/Yaolinwang/AITD) ⭐ 215 | 🐛 3 | 🌐 Python | 📅 2026-04-29 - "AI Trading Agent for Everyone"; multi-agent project designed for retail users.
* [flash131307/multi-agent-investment](https://github.com/flash131307/multi-agent-investment) ⭐ 201 | 🐛 1 | 🌐 Python | 📅 2026-03-26 - Multi-agent equity-research system that lets LLM agents gather evidence, then uses a separate math layer to produce BUY / NEUTRAL / SELL. <a id="agents-oracle3"></a>
* [liangdabiao/autogen-financial-analysis](https://github.com/liangdabiao/autogen-financial-analysis) ⭐ 155 | 🐛 0 | 🌐 Python | 📅 2025-09-17 - Microsoft AutoGen-based multi-agent financial-analysis system; VaR / Monte Carlo / factor models / visualization integration.
* [Ganador1/FenixAI\_tradingBot](https://github.com/Ganador1/FenixAI_tradingBot) ⭐ 145 | 🐛 0 | 🌐 Python | 📅 2026-08-08 - LangGraph + Ollama + CrewAI autonomous trading agent; local-LLM first.
* [ryan-yuuu/crypto-trading-arena](https://github.com/ryan-yuuu/crypto-trading-arena) ⭐ 126 | 🐛 0 | 🌐 Python | 📅 2026-07-08 - Open-source crypto-trading arena; Claude / Claude Code agents compete head-to-head on live crypto data.
* [FareedKhan-dev/multi-agent-trading-system](https://github.com/FareedKhan-dev/multi-agent-trading-system) ⭐ 114 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2025-09-04 - "Deep Thinking Trading System" tutorial implementation; beginner-friendly multi-agent example design.
* [Tanglumy/Finance-Bro](https://github.com/Tanglumy/Finance-Bro) ⭐ 111 | 🐛 0 | 🌐 Python | 📅 2025-11-08 - Persona-styled finance "bro" trading-and-investment agent; uses the persona as the main interaction style.

> \[!NOTE]
> Also useful here: [guangxiangdebizi/TradingAgents-MCPmode](#mcps-tradingagents-mcpmode) turns TradingAgents-style research into MCP tools. The full entry is in MCPs · Research tools / analysis.

> Also see: [chrisworsey55/atlas-gic](#agents-atlas-gic) is listed under single-agent traders, but it is relevant here because it replaces debate with continuous self-research.

<a id="agents-single-agent"></a>

### Single-agent end-to-end traders

<a id="agents-ai-hedge-fund"></a>

* [virattt/ai-hedge-fund](https://github.com/virattt/ai-hedge-fund) ⭐ 62,854 | 🐛 164 | 🌐 Python | 📅 2026-08-07 - Widely forked LLM-driven equity-trading repo; analyst personas (Buffett / Munger / Cathie Wood) propose, the portfolio manager decides.
* [NoFxAiOS/nofx](https://github.com/NoFxAiOS/nofx) ⭐ 12,712 | 🐛 518 | 🌐 Go | 📅 2026-07-30 - Self-hosted LLM trading terminal; models decide and explain while a Go runtime enforces hard risk limits across nine exchanges. <a id="agents-atlas-gic"></a>
* [TraderAlice/OpenAlice](https://github.com/TraderAlice/OpenAlice) ⭐ 6,508 | 🐛 29 | 🌐 TypeScript | 📅 2026-08-14 - "Your one-person Wall Street"; single agent covering research → entry → hold → exit; Claude Agent SDK + Trading-as-Git approval workflow + cross-asset UTA account design. <a id="agents-nofx"></a>
* [chrisworsey55/atlas-gic](https://github.com/chrisworsey55/atlas-gic) ⭐ 2,080 | 🐛 3 | 🌐 Python | 📅 2026-05-27 - General Intelligence Capital's self-improving trading agent; focuses on continuous self-research rather than agent debate.
* [alsk1992/CloddsBot](https://github.com/alsk1992/CloddsBot) ⭐ 686 | 🐛 20 | 🌐 TypeScript | 📅 2026-06-26 - Open-source AI trader across 1000+ markets, including Polymarket, Kalshi, Binance, Hyperliquid, Solana, and several EVM chains.
* [Gajesh2007/ai-trading-agent](https://github.com/Gajesh2007/ai-trading-agent) ⭐ 538 | 🐛 2 | 🌐 Python | 📅 2025-10-27 - AI trading agent on Hyperliquid; single-LLM-driven execution; shows direct Hyperliquid integration.
* [danilobatson/ai-trading-agent-gemini](https://github.com/danilobatson/ai-trading-agent-gemini) ⭐ 309 | 🐛 0 | 🌐 TypeScript | 📅 2026-01-05 - LunarCrush social-sentiment + Google Gemini crypto-trading agent; built with Next.js 15, Inngest, and Supabase.
* [kweinmeister/agentic-trading](https://github.com/kweinmeister/agentic-trading) ⭐ 251 | 🐛 6 | 🌐 Python | 📅 2026-07-27 - Trading-workflow example built on Google ADK + A2A interop; an alternative implementation outside LangGraph.
* [hkirat/ai-trading-agent](https://github.com/hkirat/ai-trading-agent) ⭐ 176 | 🐛 4 | 🌐 TypeScript | 📅 2025-11-02 - "Trade using LLMs"; minimal TypeScript demo from Harkirat Singh; common on-ramp for TS learners.

<a id="agents-research-copilots"></a>

### Research / equity-research copilots

* [ZhuLinsen/daily\_stock\_analysis](https://github.com/ZhuLinsen/daily_stock_analysis) ⭐ 62,894 | 🐛 47 | 🌐 Python | 📅 2026-08-14 - Daily LLM-driven stock-screening dashboard; multi-channel push (WeChat / Feishu / Telegram / Discord / Slack / email); 11 built-in strategies + agent stock-Q\&A; deploy-by-GitHub-Actions.
* [TNT-Likely/PanWatch](https://github.com/TNT-Likely/PanWatch) ⭐ 783 | 🐛 53 | 🌐 Python | 📅 2026-08-12 - PanWatch / "盯盘侠"; AI-driven stock-monitoring assistant; multi-account positions + agent analysis + PWA mobile.
* [AmadeusGB/alpha-arena](https://github.com/AmadeusGB/alpha-arena) ⭐ 626 | 🐛 8 | 🌐 Python | 📅 2025-10-20 - Live AI-agent competition and research platform; uses real-market conditions to improve agents.
* [YoungCan-Wang/WyckoffTradingAgent](https://github.com/YoungCan-Wang/WyckoffTradingAgent) ⭐ 566 | 🐛 5 | 🌐 Python | 📅 2026-08-14 - AI stock-analysis assistant for A/HK/US equities; uses Wyckoff price-volume logic and ships CLI, web, and MCP tools.
* [HKUSTDial/DeepEar](https://github.com/HKUSTDial/DeepEar) ⭐ 270 | 🐛 4 | 🌐 Python | 📅 2026-04-16 - DeepEar / "顺风耳"; HKUSTDial's open-source deep-research and signal-tracking framework; joint multimodal news + price tracking.
* [kamathhrishi/finance-agent](https://github.com/kamathhrishi/finance-agent) ⭐ 139 | 🐛 2 | 🌐 Python | 📅 2026-06-19 - Earnings-call / SEC-filing / news Q\&A agent; clean RAG-over-disclosures implementation.

> Also relevant: [ginlix-ai/LangAlpha](#agents-langalpha) and [oficcejo/aiagents-stock](#agents-tradingagents) both include research-copilot screens, but their main entries stay with the multi-agent systems they belong to.

<a id="agents-real-money"></a>

### Real-money / competition experiments

<a id="agents-llm-trading-lab"></a>

* [LuckyOne7777/LLM-Trading-Lab](https://github.com/LuckyOne7777/LLM-Trading-Lab) ⭐ 7,499 | 🐛 6 | 🌐 Python | 📅 2026-06-24 - Real-money six-month experiment; ChatGPT manages a real US-equity micro-cap portfolio under strict pre-defined rules; ships with a 40-page evaluation paper.
* [wquguru/nof0](https://github.com/wquguru/nof0) ⭐ 2,750 | 🐛 15 | 🌐 Go | 📅 2025-12-07 - nof1.ai Alpha Arena reimplementation with Go backend, Next.js UI, Hyperliquid, LLM executors, backtests, leaderboards.
* [195440/nof1.ai](https://github.com/195440/nof1.ai) ⭐ 683 | 🐛 1 | 🌐 TypeScript | 📅 2026-05-15 - Open-source autonomous AI trading agent from the nof1 family; TypeScript port.
* [oficcejo/alpha-arena-okx](https://github.com/oficcejo/alpha-arena-okx) ⭐ 334 | 🐛 28 | 🌐 Python | 📅 2026-07-27 - OKX re-implementation of nof1.ai's Alpha Arena; DeepSeek / Qwen3-Max as decision-makers; useful when comparing Chinese-language nof1 projects.

> Also see: [NoFxAiOS/nofx](#agents-nofx) runs multiple LLM traders side by side with a leaderboard; its main entry stays under single-agent traders because it is first a full trading terminal.

<a id="agents-prediction-market"></a>

### Prediction-market specialists

* [ryanfrigo/kalshi-ai-trading-bot](https://github.com/ryanfrigo/kalshi-ai-trading-bot) ⭐ 570 | 🐛 0 | 🌐 Python | 📅 2026-07-06 - Grok-4-driven Kalshi prediction-market multi-agent trading system; portfolio optimization + 5-gate risk engine.
* [OctagonAI/kalshi-trading-bot-cli](https://github.com/OctagonAI/kalshi-trading-bot-cli) ⭐ 369 | 🐛 9 | 🌐 TypeScript | 📅 2026-06-25 - AI-native CLI for Kalshi and Polymarket; researches an event, estimates probability, then compares it with the live order book.
* [jvnhaoWen/PolyAgent](https://github.com/jvnhaoWen/PolyAgent) ⭐ 101 | 🐛 1 | 🌐 Python | 📅 2026-03-24 - Polymarket-focused multi-skill trading agent; focused single-venue Polymarket LLM agent.

> Also useful here: [agent-next/polymarket-paper-trader](#mcps-polymarket-paper-trader) is listed under MCPs because it is a paper-trading simulator, but it is built for AI agents.

> Also see: [YichengYang-Ethan/oracle3](#agents-oracle3) is listed with multi-agent systems above, and it is especially relevant here for multi-venue prediction-market arbitrage.

<a id="agents-benchmarks"></a>

### Benchmarks & evaluations

* [Open-Finance-Lab/AgenticTrading](https://github.com/Open-Finance-Lab/AgenticTrading) ⭐ 387 | 🐛 65 | 🌐 Python | 📅 2026-08-15 - Open-Finance-Lab's academic framework + dataset for agent-trading research.
* [HKUSTDial/DeepFund](https://github.com/HKUSTDial/DeepFund) ⭐ 291 | 🐛 0 | 🌐 Python | 📅 2026-03-18 - Multi-agent fund-investment benchmark; LLM analysts evaluate stocks in a unified trading arena with leaderboard.
* [ulab-uiuc/live-trade-bench](https://github.com/ulab-uiuc/live-trade-bench) ⭐ 164 | 🐛 14 | 🌐 Python | 📅 2026-02-17 - Live-market evaluation for trading agents; UIUC ULab's live-eval benchmark; distinct from backtest-only benchmarks.
* [vals-ai/finance-agent](https://github.com/vals-ai/finance-agent) ⭐ 153 | 🐛 6 | 🌐 Python | 📅 2026-07-21 - Finance-agent benchmark / task suite from vals-ai. <a id="agents-deepfund"></a>

<a id="agents-strategy-coding"></a>

### Strategy coding / self-improving agents

* [HammerGPT/Hyper-Alpha-Arena](https://github.com/HammerGPT/Hyper-Alpha-Arena) ⭐ 1,129 | 🐛 23 | 🌐 Python | 📅 2026-05-13 - LLM factor-research and perpetuals platform; mines and validates 86 factors with IC / ICIR, decay, backtests, and attribution.
* [Miasyster/QuantGPT](https://github.com/Miasyster/QuantGPT) ⭐ 437 | 🐛 3 | 🌐 Python | 📅 2026-05-20 - Agent-driven A-share factor research engine; 8 MCP tools span hypothesis → backtest → score → WQ BRAIN submission. *(Distinct from rnikitin/QuantGPT.)*
* [paperswithbacktest/pwb-alphaevolve](https://github.com/paperswithbacktest/pwb-alphaevolve) ⭐ 127 | 🐛 2 | 🌐 Python | 📅 2025-06-04 - DeepMind AlphaEvolve-style agent that uses an LLM to write and improve trading strategies for backtesting.

> Note: [`TauricResearch/Trading-R1`](https://github.com/TauricResearch/Trading-R1) ⭐ 472 | 🐛 1 | 📅 2025-09-15 is not listed yet because its terminal has not launched. It can be added once the project is publicly usable.

<a id="mcps"></a>

## MCPs

<p align="center">
  <img src="assets/section-mcps.png" alt="MCPs section header" width="760" />
</p>

MCPs are servers that let an agent call external tools through the Model Context Protocol. In this list, they mostly cover market data, broker or exchange actions, research tools, and backtesting services.

> \[!NOTE]
> Same author to compare: `guangxiangdebizi/` maintains [FinanceMCP](#mcps-financemcp) for data access and [TradingAgents-MCPmode](#mcps-tradingagents-mcpmode) for TradingAgents-style research tools. They solve different problems, so they stay in separate sections.

<a id="mcps-market-data"></a>

### Market data / data providers

<a id="mcps-financial-datasets"></a>

* [financial-datasets/mcp-server](https://github.com/financial-datasets/mcp-server) ⭐ 2,277 | 🐛 14 | 🌐 Python | 📅 2025-06-05 - Financial Datasets' first-party MCP; US-equity + crypto fundamentals (3 statements + ratios) + prices + news.
* [6551Team/opennews-mcp](https://github.com/6551Team/opennews-mcp) ⭐ 2,096 | 🐛 4 | 🌐 Python | 📅 2026-08-13 - 84+ news-source aggregation (Bloomberg / Reuters / FT / CoinDesk and more) + AI impact-scoring / trading-signal + WebSocket streaming.
* [chengzuopeng/stock-sdk](https://github.com/chengzuopeng/stock-sdk) ⭐ 1,846 | 🐛 3 | 🌐 TypeScript | 📅 2026-08-07 - Zero-dependency TypeScript stock-data SDK with built-in MCP for A/H/US equities and funds via browser, Node.js, CLI, Claude Code, or Codex.
* [guangxiangdebizi/FinanceMCP](https://github.com/guangxiangdebizi/FinanceMCP) ⭐ 645 | 🐛 4 | 🌐 TypeScript | 📅 2026-08-13 - Tushare + Binance MCP spanning A-shares / HK / US / funds / bonds / macro / stablecoins / crypto / financial news.
* [saidsurucu/borsa-mcp](https://github.com/saidsurucu/borsa-mcp) ⭐ 639 | 🐛 1 | 🌐 Python | 📅 2026-08-07 - Turkish BIST + US-equity + fund data MCP serving regional markets outside China and the US.
* [elsejj/mcp-cn-a-stock](https://github.com/elsejj/mcp-cn-a-stock) ⭐ 461 | 🐛 6 | 🌐 Python | 📅 2025-12-15 - A-share-only data MCP; single-market deep coverage instead of multi-source aggregation.
* [BlockRunAI/blockrun-mcp](https://github.com/BlockRunAI/blockrun-mcp) ⭐ 425 | 🐛 3 | 🌐 TypeScript | 📅 2026-08-13 - Real-time data MCP with pay-per-call x402 payments; covers search, research, quotes, crypto, X, and Twitter. <a id="mcps-financemcp"></a>
* [aahl/mcp-aktools](https://github.com/aahl/mcp-aktools) ⭐ 390 | 🐛 0 | 🌐 Python | 📅 2026-03-26 - Stock and crypto data MCP built on akshare / aktools; broad market-data coverage through the AKShare ecosystem.
* [massive-com/mcp\_massive](https://github.com/massive-com/mcp_massive) ⭐ 380 | 🐛 7 | 🌐 Python | 📅 2026-06-11 - Massive (formerly Polygon.io) first-party MCP; multi-asset market-data coverage.
* [stefanoamorelli/sec-edgar-mcp](https://github.com/stefanoamorelli/sec-edgar-mcp) ⭐ 348 | 🐛 37 | 🌐 Python | 📅 2026-08-12 - SEC EDGAR MCP; 10-K / 10-Q / 8-K / insider trades / filings reader; common filings entry across awesome-lists.
* [Alex2Yang97/yahoo-finance-mcp](https://github.com/Alex2Yang97/yahoo-finance-mcp) ⭐ 340 | 🐛 10 | 🌐 Python | 📅 2026-03-23 - Full-feature Yahoo Finance MCP; historical prices + fundamentals + option chains + news; Yahoo wrapper.
* [zwldarren/akshare-one-mcp](https://github.com/zwldarren/akshare-one-mcp) ⭐ 221 | 🐛 8 | 🌐 Python | 📅 2026-03-14 - A-share data MCP backed by the AKShare-One normalizer; an alternative implementation within the AKShare ecosystem.
* [daniel3303/Equibles](https://github.com/daniel3303/Equibles) ⭐ 196 | 🐛 35 | 🌐 C# | 📅 2026-08-14 - Self-hosted finance data hub; syncs public SEC/FRED/Yahoo/FINRA/CFTC/CBOE data to PostgreSQL and serves it via MCP.
* [narumiruna/yfinance-mcp](https://github.com/narumiruna/yfinance-mcp) ⭐ 178 | 🐛 0 | 🌐 Python | 📅 2026-08-10 - Minimal yfinance MCP; a lightweight Yahoo Finance data option.
* [OctagonAI/octagon-mcp-server](https://github.com/OctagonAI/octagon-mcp-server) ⭐ 146 | 🐛 4 | 🌐 TypeScript | 📅 2026-07-09 - MCP for filings, earnings calls, financials, stock data, private-market deals, and web research.
* [imbenrabi/Financial-Modeling-Prep-MCP-Server](https://github.com/imbenrabi/Financial-Modeling-Prep-MCP-Server) ⭐ 141 | 🐛 3 | 🌐 TypeScript | 📅 2026-07-02 - FMP MCP with 250+ tools for fundamentals, market intelligence, and ETFs.
* [LLMQuant/data-mcp](https://github.com/LLMQuant/data-mcp) ⭐ 67 | 🐛 1 | 🌐 TypeScript | 📅 2026-08-08 - LLMQuant Data's official MCP server, positioned as the "knowledge harness for AI-native finance"; covers semantic search over a 50k+ quant wiki and 1.2k+ research papers, US equity OHLCV + dividends/splits, crypto klines & snapshots (Binance Spot), 50+ curated macro indicators (FRED, etc.), SEC 10-K/10-Q full-text browse & read, and three-way 13F institutional holdings queries (manager → holdings / ticker → holders / top managers).

<a id="mcps-brokerage"></a>

### Brokerage / exchange trading

<a id="mcps-alpaca"></a>

* [koreainvestment/open-trading-api](https://github.com/koreainvestment/open-trading-api) ⭐ 1,562 | 🐛 40 | 🌐 Python | 📅 2026-07-28 - Korea Investment & Securities official SDK; includes a Trading MCP, strategy builder, and backtester.
* [alpacahq/alpaca-mcp-server](https://github.com/alpacahq/alpaca-mcp-server) ⭐ 917 | 🐛 27 | 🌐 Python | 📅 2026-08-10 - Alpaca's official MCP for market data plus paper or live trading in equities, ETFs, options, and crypto. *(← used by: [tradermonty/claude-trading-skills](#skills-claude-trading-skills), [staskh/trading\_skills](#skills-trading-skills), [huygiatrng/AlpacaTradingAgent](#agents-tradingagents).)* <a id="mcps-kraken-cli"></a>
* [ariadng/metatrader-mcp-server](https://github.com/ariadng/metatrader-mcp-server) ⭐ 714 | 🐛 27 | 🌐 Python | 📅 2026-03-28 - Representative MT5 MCP; lets LLMs trade through any MetaTrader 5 broker; MCP connector for a major retail-forex platform.
* [krakenfx/kraken-cli](https://github.com/krakenfx/kraken-cli) ⭐ 684 | 🐛 0 | 🌐 Rust | 📅 2026-08-07 - Kraken's official AI-native CLI with an embedded MCP; covers crypto, xStocks, forex, derivatives, paper trading, and bundled SKILL.md packs. <a id="mcps-koreainvestment"></a>
* [okx/agent-trade-kit](https://github.com/okx/agent-trade-kit) ⭐ 401 | 🐛 15 | 🌐 TypeScript | 📅 2026-07-29 - OKX official MCP for spot, perpetuals, futures, options, and grid bots.
* [code-rabi/interactive-brokers-mcp](https://github.com/code-rabi/interactive-brokers-mcp) ⭐ 209 | 🐛 8 | 🌐 JavaScript | 📅 2026-07-21 - Alternative IBKR MCP in TS / JS; complements rcontesti's Python build.
* [Qoyyuum/mcp-metatrader5-server](https://github.com/Qoyyuum/mcp-metatrader5-server) ⭐ 208 | 🐛 3 | 🌐 Python | 📅 2026-08-10 - Alternative MT5 MCP for quotes, trading, and history; uses MCP resources as well as tools.
* [rcontesti/IB\_MCP](https://github.com/rcontesti/IB_MCP) ⭐ 139 | 🐛 4 | 🌐 Python | 📅 2025-10-23 - Representative IBKR MCP; exposes Interactive Brokers TWS / Gateway as MCP tools; aimed at professional-broker workflows.
* [taylorwilsdon/quantconnect-mcp](https://github.com/taylorwilsdon/quantconnect-mcp) ⭐ 116 | 🐛 3 | 🌐 Python | 📅 2025-08-24 - Independent QuantConnect MCP focused on strategy research and workflow automation.

> Also useful for Skills readers: [krakenfx/kraken-cli](#mcps-kraken-cli) includes 50 bundled SKILL.md packages. The main entry is here because it is primarily an exchange trading tool.

<a id="mcps-research-tools"></a>

### Research tools / analysis

* [mnemox-ai/tradememory-protocol](https://github.com/mnemox-ai/tradememory-protocol) ⭐ 1,410 | 🐛 2 | 🌐 Python | 📅 2026-08-11 - Memory MCP for AI trading agents; records decision rationale, outcomes, and review evidence with 17 MCP tools and 35+ REST endpoints. <a id="mcps-tradingagents-mcpmode"></a>
* [wshobson/maverick-mcp](https://github.com/wshobson/maverick-mcp) ⭐ 644 | 🐛 14 | 🌐 Python | 📅 2026-08-05 - Personal stock-analysis MCP for fundamentals, technical indicators, and screening.
* [QuantMLResearch/AI-Kline](https://github.com/QuantMLResearch/AI-Kline) ⭐ 340 | 🐛 5 | 🌐 Python | 📅 2025-08-06 - Stock-analysis tool combining classic technical analysis, AI prediction, and MCP access.
* [guangxiangdebizi/TradingAgents-MCPmode](https://github.com/guangxiangdebizi/TradingAgents-MCPmode) ⭐ 332 | 🐛 7 | 🌐 Python | 📅 2025-11-22 - TradingAgents refactored as MCP tools for multi-agent equity research.
* [wbsu2003/stock-scanner-mcp](https://github.com/wbsu2003/stock-scanner-mcp) ⭐ 243 | 🐛 7 | 🌐 Python | 📅 2025-07-03 - Stock scanner MCP for prices, scoring, technical reports, and AI summaries.

> Also relevant: [dragon1086/prism-insight](#agents-prism-insight) is listed under Agents; this section mentions it because it has built-in MCP support for research.

<a id="mcps-tradingview"></a>

### TradingView bridge

* [atilaahmettaner/tradingview-mcp](https://github.com/atilaahmettaner/tradingview-mcp) ⭐ 3,964 | 🐛 8 | 🌐 Python | 📅 2026-08-07 - 30+-tool TradingView MCP; 6 backtest strategies + Reddit sentiment + news + multi-exchange; many tools work without an API key.

<a id="mcps-prediction-market"></a>

### Prediction markets

<a id="mcps-polymarket"></a>

* [caiovicentino/polymarket-mcp-server](https://github.com/caiovicentino/polymarket-mcp-server) ⭐ 634 | 🐛 4 | 🌐 Python | 📅 2026-07-30 - 45-tool Polymarket MCP; real-time monitoring and explicit order-safety guards. <a id="mcps-polymarket-paper-trader"></a>
* [agent-next/polymarket-paper-trader](https://github.com/agent-next/polymarket-paper-trader) ⭐ 372 | 🐛 7 | 🌐 Python | 📅 2026-08-15 - Polymarket paper-trading simulator; MCP server + real-time order book + strategy backtesting; built for AI agents.

<a id="mcps-backtesting"></a>

### Strategy / backtesting platforms

* [whchien/ai-trader](https://github.com/whchien/ai-trader) ⭐ 995 | 🐛 6 | 🌐 Python | 📅 2026-03-28 - Backtrader-based framework with 20+ strategies, multi-market support, CLI tools, and an embedded MCP for agent workflows.

<a id="skills"></a>

## Skills

<p align="center">
  <img src="assets/section-skills.png" alt="Skills section header" width="760" />
</p>

Skills are reusable instructions and workflows for Claude Code or other agent systems. They help an agent repeat a trading task reliably, such as researching a stock, checking options, backtesting a strategy, or managing a portfolio. When a Skill is designed to work with a listed MCP, the entry shows `→ pairs with`.

<a id="skills-equity-research"></a>

### Equity research

<a id="skills-claude-trading-skills"></a>

* [xbtlin/ai-berkshire](https://github.com/xbtlin/ai-berkshire) ⭐ 15,547 | 🐛 31 | 🌐 Python | 📅 2026-08-14 - Value-investing research framework for Claude Code / Codex; combines four investor playbooks with multi-agent analysis.
* [himself65/finance-skills](https://github.com/himself65/finance-skills) ⭐ 3,162 | 🐛 5 | 🌐 JavaScript | 📅 2026-08-05 - Skill pack for multiple asset classes, covering valuation, earnings review, option payoffs, ETF checks, liquidity, social research, and geopolitical-risk analysis.
* [RKiding/Awesome-finance-skills](https://github.com/RKiding/Awesome-finance-skills) ⭐ 2,775 | 🐛 8 | 🌐 Python | 📅 2026-03-29 - Alphaear Skill suite for news, stocks, sentiment, prediction, signal tracking, logic visualization, reporting, and search.
* [tradermonty/claude-trading-skills](https://github.com/tradermonty/claude-trading-skills) ⭐ 2,644 | 🐛 24 | 🌐 Python | 📅 2026-08-13 - Large Skill pack for US-equity investors, covering market analysis, breadth, regimes, screening methods, options, Alpaca portfolio management, and research workflows. *(→ pairs with: [alpacahq/alpaca-mcp-server](#mcps-alpaca).)* <a id="skills-finance-skills"></a>
* [quant-sentiment-ai/claude-equity-research](https://github.com/quant-sentiment-ai/claude-equity-research) ⭐ 689 | 🐛 0 | 🌐 Python | 📅 2026-08-11 - Claude Code research Skill for buy / sell / hold reports using fundamentals, technicals, option flow, insider activity, and sector context.
* [monarchjuno/tradingcodex](https://github.com/monarchjuno/tradingcodex) ⭐ 359 | 🐛 0 | 🌐 Python | 📅 2026-07-24 - Codex-native investment workflow team for research, portfolio work, and trading-oriented analysis. <a id="skills-alphaear"></a>
* [JoelLewis/finance\_skills](https://github.com/JoelLewis/finance_skills) ⭐ 169 | 🐛 4 | 🌐 Python | 📅 2026-07-18 - Claude Code financial-services Skill pack; 84 skills across investment management, compliance, advisory workflows, trading operations, and portfolio reporting.

> Also useful here: [HKUDS/Vibe-Trading](#agents-vibe-trading) and [ginlix-ai/LangAlpha](#agents-langalpha) both include bundled Skills. Their main entries stay under Agents because they are full agent workspaces, not just Skill packs.

<a id="skills-crypto"></a>

### Crypto / DeFi / on-chain

* [GMGNAI/gmgn-skills](https://github.com/GMGNAI/gmgn-skills) ⭐ 446 | 🐛 28 | 🌐 TypeScript | 📅 2026-08-14 - GMGN Agent Skills for querying tokens, wallets, and market data, and executing on-chain trades across Solana, BSC, and Base.
* [okx/onchainos-skills](https://github.com/okx/onchainos-skills) ⭐ 322 | 🐛 15 | 🌐 Rust | 📅 2026-08-14 - OKX official Skills for OnchainOS, covering wallets, token discovery, quotes, DEX swaps, and transaction broadcasting.
* [Polymarket/agent-skills](https://github.com/Polymarket/agent-skills) ⭐ 181 | 🐛 4 | 📅 2026-02-19 - First-party Polymarket Agent Skill for auth, orders, market data, WebSockets, bridging, and gasless flows.
* [okx/agent-skills](https://github.com/okx/agent-skills) ⭐ 161 | 🐛 7 | 🌐 Shell | 📅 2026-07-22 - OKX bilingual Skills repo with contribution, review, and security guidance; companion to onchainos-skills.

<a id="skills-strategy-coding"></a>

### Strategy coding & backtesting

<a id="skills-vectorbt-backtesting"></a>

* [MobiusQuant/OpenMobius-skill](https://github.com/MobiusQuant/OpenMobius-skill) ⭐ 630 | 🐛 0 | 🌐 Python | 📅 2026-07-06 - ICT / SMC trading-knowledge Skill for Claude Code, Codex, OpenClaw, and Hermes; includes curated knowledge cards, real-time market data, indicators, and chart generation.
* [Superior-Trade/superior-skills](https://github.com/Superior-Trade/superior-skills) ⭐ 213 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-13 - Agent Skills and tool schemas for building, backtesting, and deploying Hyperliquid trading strategies.
* [marketcalls/vectorbt-backtesting-skills](https://github.com/marketcalls/vectorbt-backtesting-skills) ⭐ 191 | 🐛 3 | 🌐 Python | 📅 2026-07-12 - Skill for vectorbt backtesting with setup, backtest, optimization, quick stats, strategy comparison, and reusable strategy templates.

<a id="skills-brokerage"></a>

### Brokerage execution & portfolio

<a id="skills-trading-skills"></a>

* [koreal6803/finlab-ai](https://github.com/koreal6803/finlab-ai) ⭐ 411 | 🐛 1 | 📅 2026-08-14 - Taiwan-equity CLI Skill for strategy discovery, backtesting, and feature engineering with FinLab data and ready-made strategy examples.
* [staskh/trading\_skills](https://github.com/staskh/trading_skills) ⭐ 332 | 🐛 18 | 🌐 Python | 📅 2026-08-10 - Skill pack for option traders, covering market data, analysis, scanners, portfolio work, reports, IBKR integration, and MCP tools. *(→ pairs with: [alpacahq/alpaca-mcp-server](#mcps-alpaca), [rcontesti/IB\_MCP](https://github.com/rcontesti/IB_MCP) ⭐ 139 | 🐛 4 | 🌐 Python | 📅 2025-10-23.)*
* [second-state/fintool](https://github.com/second-state/fintool) ⭐ 313 | 🐛 1 | 🌐 Rust | 📅 2026-05-19 - Rust CLI suite for agentic trading and market intelligence; exchange-specific tools for Hyperliquid / Binance / Coinbase / OKX / Polymarket plus quotes, news, SEC filings, and backtests.

> Also useful here: [krakenfx/kraken-cli](#mcps-kraken-cli) includes SKILL.md packages for crypto, xStocks, forex, and derivatives. The full entry is under MCPs because Kraken CLI is mainly an exchange trading tool.

<a id="resources"></a>

## Resources

<a id="resources-papers"></a>

### Papers

> Included here: papers that directly introduce or explain a project listed here. For a broader finance-LLM paper, model, and dataset list, see [`DataArcTech/Awesome-FinLLMs`](https://github.com/DataArcTech/Awesome-FinLLMs) ⭐ 67 | 🐛 0 | 📅 2026-06-23.

* [FinRobot: Open-Source AI Agent Platform for Financial Analysis](https://arxiv.org/abs/2405.14767) - AI4Finance Foundation, arXiv 2405.14767 (2024). Early academic finance-AI agent platform; multimodal analyst agents tied to the FinGPT model line. [paper](https://arxiv.org/abs/2405.14767) · [code](https://github.com/AI4Finance-Foundation/FinRobot) ⭐ 7,784 | 🐛 72 | 🌐 Jupyter Notebook | 📅 2026-07-27
* [LLM-Trading-Lab: Six-Month Real-Money ChatGPT Micro-Cap Experiment](https://github.com/LuckyOne7777/LLM-Trading-Lab) ⭐ 7,499 | 🐛 6 | 🌐 Python | 📅 2026-06-24 - Lucky One, 2025; ships with a 40-page evaluation paper. Forward-only audit of ChatGPT managing a real US-equity micro-cap portfolio for six months under strict pre-defined rules. [paper / repo](https://github.com/LuckyOne7777/LLM-Trading-Lab) ⭐ 7,499 | 🐛 6 | 🌐 Python | 📅 2026-06-24 · [code](#agents-llm-trading-lab)
* [TradingAgents: Multi-Agents LLM Financial Trading Framework](https://arxiv.org/abs/2412.20138) - Tauric Research team, arXiv 2412.20138 (2024). Introduces the multi-agent debate decision framework: analyst team + bull/bear researcher debate + trader + risk control + portfolio manager. [paper](https://arxiv.org/abs/2412.20138) · [code](#agents-tradingagents)
* [Time Travel is Cheating: Going Live with DeepFund for Real-Time Fund Investment Benchmarking](https://arxiv.org/abs/2505.11065) - HKUSTDial, arXiv 2505.11065 (2025). Multi-agent fund-investment benchmark with LLM analysts and a trading arena leaderboard. [paper](https://arxiv.org/abs/2505.11065) · [code](#agents-deepfund)

> For broader finance-LLM papers, models, and datasets, see [`DataArcTech/Awesome-FinLLMs`](https://github.com/DataArcTech/Awesome-FinLLMs) ⭐ 67 | 🐛 0 | 📅 2026-06-23. This list stays focused on usable agent, MCP, and Skill projects.

<a id="resources-learn"></a>

### Learn

> Included here: public talks, courses, and long-form posts about LLM-driven trading. We skip generic LLM tutorials, generic finance tutorials, and paid courses without a public artifact.

* [Tauric Research GitHub Org](https://github.com/TauricResearch) - Tauric Research, ongoing 2024–2026. Official org behind the TradingAgents framework; public README / docs / companion technical reports (arXiv 2412.20138 / 2509.11420); a good place to learn how multi-agent trading systems are built. [link](https://github.com/TauricResearch)
* [AI4Finance Foundation GitHub Org](https://github.com/AI4Finance-Foundation) - AI4Finance Foundation, ongoing 2022–2026. Official org behind the FinRobot / FinGPT / FinRL line; ProjectShare / tutorial notebooks / paper companion code; a good place to learn academic finance-AI agents. [link](https://github.com/AI4Finance-Foundation)

> Note: the v0.1 Learn section is intentionally short. Future updates can add talks, courses, podcasts, and conference sessions as they become useful to readers.

<a id="contributing"></a>

## Contributing

We welcome community contributions: new entries, removal of dead links, and discussion on sub-category boundaries. Start with [CONTRIBUTING.md](CONTRIBUTING.md) (or [CONTRIBUTING.zh-CN.md](CONTRIBUTING.zh-CN.md) in Chinese); the guide puts the AI-native review path, quality bar, submission format, `awesome-lint` check, and bilingual-PR rule in one place. New entries are smoothest via the [Issue: add entry](.github/ISSUE_TEMPLATE/add-entry.md) template; removals via the [Issue: remove entry](.github/ISSUE_TEMPLATE/remove-entry.md) template.

<a id="related-awesome-lists"></a>

## Related awesome lists

* [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) ⭐ 92,332 | 🐛 2,963 | 📅 2026-08-03 - Broad MCP server directory; use this list when you only want trading, research, data, and execution tools.
* [wilsonfreitas/awesome-quant](https://github.com/wilsonfreitas/awesome-quant) ⭐ 28,772 | 🐛 59 | 🌐 HTML | 📅 2026-08-15 - Classical quant-library list; useful, but not the focus here.
* [georgezouq/awesome-ai-in-finance](https://github.com/georgezouq/awesome-ai-in-finance) ⭐ 6,400 | 🐛 30 | 📅 2026-08-04 - Traditional AI-in-finance list for deep learning, reinforcement learning, and time-series work.
* [wangzhe3224/awesome-systematic-trading](https://github.com/wangzhe3224/awesome-systematic-trading) ⭐ 4,918 | 🐛 2 | 🌐 HTML | 📅 2026-08-14 - Systematic-trading list for the broader non-agent trading tools.
* [Tom-roujiang/Awesome-LLM-Quantitative-Trading-Papers](https://github.com/Tom-roujiang/Awesome-LLM-Quantitative-Trading-Papers) ⭐ 226 | 🐛 1 | 📅 2026-07-24 - Curated LLM quantitative-trading paper list; complements this repo's application-layer focus with broader research coverage.
* [DataArcTech/Awesome-FinLLMs](https://github.com/DataArcTech/Awesome-FinLLMs) ⭐ 67 | 🐛 0 | 📅 2026-06-23 - Comprehensive finance-LLM paper / model / dataset list (complementary to this list — they cover base models and papers, we cover the application-layer agents · MCPs · Skills).

<a id="maintained-by"></a>

## Maintained by

<div align="center">
  <img src="assets/llmquant-logo.svg" alt="LLMQuant" width="72" />
  <br/>
  <strong><a href="https://llmquant.com">LLMQuant</a></strong>
  <br/>
  <sub>Open-source community for AI, LLMs, and quantitative finance.</sub>
  <br/><br/>
  <a href="https://llmquant.com">Website</a> ·
  <a href="https://github.com/LLMQuant">GitHub</a> ·
  <a href="https://linkedin.com/company/llmquant">LinkedIn</a>
</div>

The maintainer team reviews new entries and category changes.

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=LLMQuant/awesome-trading-agents\&type=Date)](https://www.star-history.com/#LLMQuant/awesome-trading-agents\&Date)

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-15._
