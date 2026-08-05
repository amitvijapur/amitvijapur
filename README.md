<div align="center">

# AMIT

**CS @ Durham · Quant Systems · Agent Infrastructure · Open Source**

[![Visitors](https://visitor-badge.laobi.icu/badge?page_id=amitvijapur.amitvijapur)](https://github.com/amitvijapur)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-amitvijapur-0A66C2?style=flat&logo=linkedin)](https://linkedin.com/in/amitvijapur)
[![Substack](https://img.shields.io/badge/Substack-mitsterr-FF6719?style=flat&logo=substack&logoColor=white)](https://substack.com/@mitsterr)
[![Email](https://img.shields.io/badge/Email-vijapuramit@gmail.com-EA4335?style=flat&logo=gmail)](mailto:vijapuramit@gmail.com)

</div>

---

> *I build trading systems, agentic infrastructure, and the routing layers that decide who should do the work — a model, a machine, or a person.*

---

## ⚡ featured

### [warrant](https://github.com/amitvijapur/warrant) · [live demo →](https://warrant-agentos.netlify.app)

> 🥇 **Top 5 of 53** — GenAI Fund Agentic AI Build Week 2026, Founder Mode track, built solo

**An operating system for a workforce of humans and AI agents.** It decides *who should do each piece of work* — an AI agent, a human, or an agent that proposes and a human who approves. Every task is routed through an interpretable score, every irreversible action is gated behind a signed human approval, and the system learns which workers to trust from judged, human-confirmed outcomes.

Reputation buys autonomy on reversible work, and buys nothing on irreversible work.

`Next.js 16` · `TypeScript` · `Supabase` · `OpenAI` · `Langfuse` · 60 tests passing

---

### [cortex](https://github.com/amitvijapur/cortex)

**A meta-router for Claude Code.** It sits above every workflow system in the stack and decides, per task, which system, which specialist, and which effort tier — then logs the decision and learns from the outcome.

A friendly response to Karpathy's LLM Council: multi-model voting is one useful tool, but routing is the harder problem.

`Python` · `Shell` · `Markdown`

---

### [backtesting-engine](https://github.com/amitvijapur/backtesting-engine)

**A modular backtesting engine in Rust**, built on [Polars](https://pola.rs/). Strategies are swappable behind a `Strategy` trait, execution is realistic (next-bar fills, commission, slippage), and it ships with Kelly position sizing, grid-search parameter optimisation, and walk-forward validation to catch overfitting. Includes a Rust-versus-pandas benchmark.

`Rust` · `Polars` · `clap`

---

### [btc-trading-simulator](https://github.com/amitvijapur/btc-trading-simulator)

**A live Bitcoin trading simulator.** Streams real-time price from the Binance WebSocket API, computes SMA, EMA and RSI on the client, and simulates market and limit orders with full portfolio and P&L tracking.

`Node.js` · `Express` · `vanilla JS` · `Chart.js`

---

## 🧰 also open source

| repo | what it does |
|---|---|
| [orchestrator](https://github.com/amitvijapur/orchestrator) | Prompt generator and router for Claude Code — classifies a task, calibrates effort, picks the system and the specialist, and writes the prompt |
| [skill-auditor](https://github.com/amitvijapur/skill-auditor) | Audits a candidate Claude skill for redundancy, routing conflicts and trigger collisions *before* you install it |
| [claude-skills](https://github.com/amitvijapur/claude-skills) | The hub repo — every skill above, cloneable in one go |

---

## 🔧 merged into other people's code

Five PRs merged in three weeks, all into tools I use daily. Each one started as a bug I hit myself, was reproduced before it was fixed, and shipped with regression tests.

| project | ★ | what landed |
|---|---|---|
| [Understand-Anything](https://github.com/Egonex-AI/Understand-Anything/pull/598) | 77.5k | A `PostToolUse` hook read its payload from a stale env var instead of stdin, so it silently saw nothing |
| [Scrapling](https://github.com/D4Vinci/Scrapling/pull/379) | 72.6k | The response cache dropped cookies on browser-engine responses, breaking session reuse |
| [last30days](https://github.com/mvanhorn/last30days-skill/pull/851) | 57.3k | A silent fallback masked YouTube transcript failures, so a broken fetch looked identical to an empty result |
| [fastmcp](https://github.com/punkpeye/fastmcp/pull/296) | 3.2k | **MCP resource subscriptions** — a new feature, shipped in `v4.8.0` |
| [toolport](https://github.com/tsouth89/toolport/pull/366) | 108 | Witsy MCP client support, credited by the maintainer in the README |

In review: two PRs into [mcp-atlassian](https://github.com/sooperset/mcp-atlassian) (★5.7k) closing a space-filter bypass across the Confluence tools. The allowlist was checked against the space you named, but not against the parent page the write actually landed under — so the page was created in a filtered space and the error only surfaced afterwards.

---

## 🏆 hackathons & build weeks

### 🥇 GenAI Fund Agentic AI Build Week 2026 — Ho Chi Minh City

**Top 5 of 53 · Founder Mode track · Problem P4, "Human-AgentOS" · built solo**

Shipped [**warrant**](https://github.com/amitvijapur/warrant) in a single build day: a closed loop for human/AI workforce allocation. A task arrives with capability requirements and a reversibility flag; a router scores every registered worker on capability match, cost, latency and evidenced reliability; irreversible actions structurally require human authority regardless of reputation; work executes for real, outcomes are judged, and the next identical task routes differently.

Simulated workload, real executions — every execution, score and posterior update is recorded in an append-only evidence log.

---

## 🛠 stack

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Solidity](https://img.shields.io/badge/Solidity-363636?style=for-the-badge&logo=solidity&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)

![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Polars](https://img.shields.io/badge/Polars-CD792C?style=for-the-badge&logo=polars&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

</div>

---

## 📐 background

**CS @ Durham University** — going into second year, deep in quant systems, algorithmic trading and agent infrastructure. Building real products alongside the degree, not after it.

Before Durham: **3rd Sergeant, Singapore Army (Military Police)** — commanded a 10-man team in high-pressure, compliance-driven environments. Learned to think in systems and manage risk before I knew what those words meant in trading.

---

## 📝 writing

I write about crypto, tokenomics, quant and emerging tech on [Substack](https://substack.com/@mitsterr).

Latest: **Crypto-Currencies & Tokenomics: Their Relevance in the Next Decade**

---

### 🎯 outside the terminal

```
long distance running  ·
street photography     ·
specialty coffee       ·
guitar                 ·
```
