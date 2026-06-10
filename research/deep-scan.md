# Deep Scan (Forensics)

The **Forensics** tab answers: **"is this token a scam / rug?"** It runs a live, server-side forensic
engine — not a client-side approximation.

## How to run it

1. Open a token in the [Token Workspace](token-workspace.md) → **Forensics** tab (the contract is
   pre-filled).
2. Press **Scan**.
3. Wait for the scan to complete (a full Pro scan is an async job — you'll see a progress bar; ~1–3 min
   for deep scans).

{% hint style="info" %}
You can also paste any contract directly into the Deep Scan box, or open it straight from a
[Degen Lab](../discover/degen-lab.md) result via **🛰️ Full Forensics**.
{% endhint %}

## What it checks

The engine produces a **9-objective** verdict, including:

* **Sybil / wallet clustering** — top-holder cohorts that are secretly one entity (shared funders,
  shared-token portfolios). See [Wallet Cluster](wallet-cluster.md) for the dedicated view.
* **Recursive funder traces** — who funded the holders, and whether they trace back to one source.
* **Holder concentration & persistence** — how tightly supply is held, and by whom over time.
* **Rug / LP risk** — liquidity, ownership, and contract-level red flags (via security providers).

The result is a **tiered verdict** (e.g. GREEN → RED) with a 9-objective breakdown so you can see *why*.

## Lite vs Pro

* **Lite** runs client-side for a fast first read.
* **Pro** runs the full server engine (deeper sybil stack: multi-layer funder trace, deployer-connection,
  per-wallet portfolio correlation). It falls back to the Lite read automatically if the server is
  unavailable or the chain isn't supported.

## Chains

EVM chains (Ethereum, Base, Arbitrum, Optimism, Polygon, **BSC**) run the full server engine; **Solana**
uses a dedicated SPL path. BSC top-holder cohorts are sourced via a fallback provider so clustering &
forensics work there too.

{% hint style="warning" %}
Forensics **reduces** rug risk — it does not eliminate it. A clean scan can still rug. Treat the verdict
as one input, not a guarantee.
{% endhint %}

---

**Next:** [Wallet Cluster →](wallet-cluster.md)
