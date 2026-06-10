# Signal-Trade

**Track → Signal-Trade** is our **public paper track record**. We trade our own signals in the open so the
edge is **shown, not just claimed**.

## What it is

When a signal fires, it's **auto-executed as a paper trade** and recorded here — entries, exits, P&L, and
running stats. Nothing is hidden or back-filled after the fact.

## How trades are run (paper-trading rules)

Uniform assumptions across every trade:

* Fixed **notional per position** and a fixed **initial capital** with a max number of concurrent
  positions.
* Each strategy documents its **entry rule, take-profit / stop, timeout and cooldown** (e.g. the
  SqueezePattern4H 4-hour k-rule with a TP/SL and a 3-bar pre-entry price-change filter).
* Fills, take-profits, stops, timeouts and cancels are applied on a schedule by the engine — no manual
  intervention.

## How to read the record

* **Win rate, profit factor, net P&L, return %** — the headline stats.
* The **equity curve** shows cumulative performance; low hit-rate / runner-carried positive skew is
  expected for this style (avg win outruns avg loss).
* Each row links back to the token's [Token Workspace](../research/token-workspace.md).

{% hint style="warning" %}
**Paper, not live.** This is a simulated track record for transparency and research. Past simulated
performance does not guarantee future results, and is not financial advice.
{% endhint %}

---

**Next:** [Private Bookmarks →](bookmarks.md)
