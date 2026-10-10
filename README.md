# Sentinel Audit — Automated Smart Contract Security Scans

**First scan is free. Prove it to yourself.**

## What it does

Paste your Solidity contract or GitHub repo URL. Get a security report in minutes. No sign-up, no sales call, no waiting weeks for an audit firm.

- **Mathematical invariant engine** — your contract is translated into equations (reentrancy, oracle freshness, access control, accounting integrity, and more), then the engine tries to break them
- **Fork-mode testing** — scans run against live mainnet state
- **Slither + Aderyn + fuzzing** in every run

## How accurate?

Straight answer: it's a machine, not a miracle. Findings are execution-checked wherever the harness allows it, and every report states its confidence level instead of pretending certainty. The engine caught a real division-by-zero griefing vector on a live protocol that manual review missed.

**Don't take our word for it. Get a free scan and see.**

## Pricing

| Tier | Price | What you get |
|------|-------|--------------|
| **Free** | $0 | 1 pasted contract — prove it works |
| **Quick** | $0.50 USDC | Repo or pasted source, 64 fuzz runs |
| **Full** | $49 USDC | Repo or pasted source, 256 fuzz runs, full report |

Payment: USDC on Base, automatic. Bots welcome — the API speaks the x402 payment standard: hit the endpoint, pay, get your report. No human in the loop.

## Get a scan

We're onboarding users directly while the public endpoint rolls out — reach out through this repo and we'll send you the API address plus your free scan.

**For bots/agents:** Submit, pay (x402 or unique-amount USDC on Base), receive report — no human interaction needed.

## Why we're different

Traditional audit firms charge $50K+ and take weeks. Other automated scanners drown you in false positives.

We built an engine that translates your contract into math, then tries to break it. When the math breaks, that's a real bug — not a guess. And when we're not sure, the report says so.

**Free scan. No excuses. Try it.**

---

*Automated findings are candidates for human review. For critical systems, combine with a professional audit.*
