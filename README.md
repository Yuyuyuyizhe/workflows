# Portfolio: June – August

---

## Frontend Patrol: Live Rooms & Products

**Legend**
**Verdicts** · 🟢 **Pass** — No violations detected in the live room or product · 🔴 **Reject** — Violations found; further action required
**Node Types** · 🧠 **LLM Node** — Large language model judgment node · 🟦 **Code Node** — Lightweight, deterministic rule execution

### Live Stream Highlights

**Durian**
> [!TIP]
> **Why replace LLM nodes with code nodes for deterministic checks?**
> LLMs struggle with precise, deterministic checks — substring matching, exact value comparisons, and other rule-based checks. Code handles these reliably, with 100% accuracy.

![Durian Live Stream](durian_live.svg)

**Pesticide**
> [!TIP]
> **When to replace LLM nodes with code nodes?**
> If deterministic rules (e.g., blacklisted keywords) can be distilled from the check logic, do so. This delivers **higher accuracy**, lower latency, and significant savings on tokens and compute.

![Pesticide Live Stream](pesticide_live.svg)

**Calligraphy**
> [!TIP]
> **Got multiple independent checks?**
> When they don't depend on one another, run them concurrently instead of sequentially. This drastically cuts overall latency.

![Calligraphy Live Stream](calligraphy_live-2.svg)

**Beef & Egg**
> [!TIP]
> **Got rules requiring two matches to trigger?**
> If a check needs both conditions to match and one is code-checkable, front-load the code node as a gatekeeper. On no match, short-circuit directly to a pass — bypassing the LLM node entirely. This cuts average latency significantly.

![Beef and Egg Live Stream](beaf_and_egg_live.svg)

### Product Showcase

**Seeds**
![Seed Product](seed_product.svg)

---

## Public Opinion Perception

### Public Opinion Filtering
![Public Opinion Filtering](public_filter.svg)

### Risk Rating
![Risk Rating](public_rank.svg)
