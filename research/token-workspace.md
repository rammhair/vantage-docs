# Token Workspace

**Research → Token** is your home base. Everything about a single token lives here.

## Searching a token

In the search box, paste any of:

* an **EVM contract** — `0x…` (40 hex), or
* a **Solana mint** — base58, or
* a **ticker** — e.g. `BTC`, `SOL` (resolved to its on-chain market where possible).

Press **Analyze**.

## The composite verdict

The headline result is a **composite score (0–100)** with a colour and a pattern label, plus a
**plain-English read**. The score fuses the analytical legs (smart-money, CEX supply, OI divergence,
holder concentration) into one number.

| Colour | Meaning |
| --- | --- |
| 🟢 Green | Bullish — markets agree, net accumulation |
| 🟡 Grey/Yellow | Neutral — no decisive edge |
| 🔴 Red | Bearish — distribution / caution |

Common **pattern labels** include *full agreement* (strongest), *strong buy*, *accumulation*,
*on-chain distribution*, *distribution*, and *neutral*.

{% hint style="info" %}
**"No backbone coverage"?** The token isn't in the **scored universe** yet (the composite needs indexed
history). That's normal for new tokens — the **live on-chain tools still work**. Either open it from
[Degen Lab](../discover/degen-lab.md), or use the Forensics / Wallet Cluster / On-Chain tabs directly.
{% endhint %}

## The tabs

Once a token is loaded, the workspace exposes tabs — each is the *single-token version* of a Discover
section:

| Tab | What it shows |
| --- | --- |
| **Overview** | The composite verdict + market snapshot. |
| **Perpetual** | Derivatives / OI-divergence read for this token. |
| **On-Chain** | Accumulation / distribution flow (this token's transfers). |
| **Wallet Cluster** | Connected top-holders — see [Wallet Cluster](wallet-cluster.md). |
| **Forensics** | Live scam / rug / LP **Deep Scan** — see [Deep Scan](deep-scan.md). |

## Tips

* **★ (star)** any token to add it to your [Private Bookmarks](../track/bookmarks.md).
* Supported chains: **Solana, Ethereum, BSC, Base, Arbitrum, Optimism, Polygon, Avalanche** (coverage
  varies per tool — on-chain forensics & clustering are EVM + Solana).
* Every analysis you run earns **[Rewards](../track/rewards.md)** points when signed in.

---

**Next:** [Deep Scan (Forensics) →](deep-scan.md)
