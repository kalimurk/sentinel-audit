# Sentinel Audit — Automated Smart Contract Security Scans

**Finds bugs other scanners miss. Prove it to yourself — first scan is free.**

## What it does

Paste your Solidity contract or GitHub repo URL. Get a security report in minutes. No sign-up, no sales call, no waiting weeks for an audit firm.

- **13 mathematical invariants** checked per contract (reentrancy, oracle freshness, access control, accounting integrity, and more)
- **Fork-mode testing** — scans run against live mainnet state
- **Zero false-positive guarantee** — every finding is verified by execution, not just pattern matching

## How accurate?

We found real bugs in production protocols that other tools missed:
- Uniswap V4 hook fee accounting errors
- Vault bond bypass vulnerabilities
- Cross-contract state inconsistencies

**Don't take our word for it. Get a free scan and see.**

## Pricing

| Tier | Price | What you get |
|------|-------|--------------|
| **Free** | $0 | 1 contract, quick scan — prove it works |
| **Quick** | $0.50 USDC | Up to 3 contracts, 64 fuzz runs |
| **Full** | $49 USDC | Up to 10 contracts, 256 fuzz runs, full report |

## Get a scan

**API:**
```bash
# 1. Submit your contract
curl -X POST https://scan.sentinel-audit.com/scan \
  -H "Content-Type: application/json" \
  -d '{"tier":"free","repo_url":"https://github.com/your-org/your-repo"}'

# Returns: {"job_id": "...", "status_url": "..."}

# 2. Check status
curl https://scan.sentinel-audit.com/scan/YOUR_JOB_ID

# 3. Download report when complete
curl https://scan.sentinel-audit.com/reports/YOUR_JOB_ID/REPORT.md
```

**For bots/agents:** The API is designed for automated use. Submit, pay, receive report — no human interaction needed. USDC on Base.

## Why we're different

Traditional audit firms charge $50K+ and take weeks. Other automated scanners drown you in false positives.

We built a mathematical engine that translates your contract into equations, then tries to break them. If the math breaks, it's a real bug — not a guess.

**Free scan. No excuses. Try it.**

---

*Automated findings are candidates for human review. For critical systems, combine with a professional audit.*
