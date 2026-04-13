# Autonomous AI Agents (The Frontier Phase)

Welcome to the Frontier. This repository introduces the first generation of "Protocol Residents"—AI Agents capable of managing the **Alex000115** library autonomously. Unlike simple scripts, these agents use reasoning loops to analyze market conditions in the Dark Pool (Repo 82), evaluate risk in the Staking Pool (Repo 89), and vote on proposals in the Forge DAO (Repo 99).

## Core Features
* **State-Aware Reasoning:** The agent queries the Master Dashboard subgraphs to understand current protocol health.
* **On-Chain Action Engine:** Utilizes Viem and private key management (via secure TEE or KMS) to sign transactions.
* **Governance Intelligence:** Analyzes DAO proposals using NLP to determine if a change aligns with the $ALEX economic model.
* **Flat Architecture:** Single-directory layout for the Agent Core, LLM Prompt Logic, and Execution Handlers.



## Logic Flow
1. **Perceive:** The Agent scans the 100 repos and their live deployments for anomalies or opportunities.
2. **Reason:** Using the LLM, it decides if a specific action (e.g., "Arbitrage between Repo 90 and Repo 30") is profitable.
3. **Approve:** The Agent checks its internal "Guardrails" (risk limits) before proceeding.
4. **Execute:** It broadcasts a multi-chain transaction and logs the result to the Portfolio Nexus (Repo 101).

## Setup
1. `npm install`
2. Configure `OPENAI_API_KEY` and `SIGNER_PRIVATE_KEY` in `.env`.
3. `node agent-start.js`
