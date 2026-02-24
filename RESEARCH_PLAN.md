# RESEARCH_PLAN.md
## Next Session Research Tasks
*Saved: 2026-02-24*

---

## TASK 1 — Find the exact sDAI bonding mechanism RH described
**Priority: High**

### What to find:
- The specific RH tweet/stream/post where he recommends sDAI bonding — exact quote, date, context
- What protocol/contract is doing the bonding (BetterBank? PulseMaker? New contract?)
- What you give: sDAI from Ethereum? psDAI from PulseChain? Both?
- What you get back: pDAI? PLS? PLSX? Discounted governance tokens? Vested?
- Vesting period / discount rate if it's an OlympusDAO-style bond
- Whether bonding is live yet or incoming

### Where to search:
- @RichardHeartWin X timeline — recent posts mentioning sDAI, bonding, DSR
- @NineIronCapital — likely covered it
- @DuRtY_Crypto — usually amplifies any RH alpha quickly
- BetterBank docs / Medium posts (betterbank.io or similar)
- PulseMaker governance portal (pulsemaker.win) — new proposals post-ESM?
- pulsechaindai.com/research — may have new entries
- pdai.net — official site may have updated post-ESM

### Key question to answer:
> Does bonding sDAI produce more total return than simply holding pDAI if the peg happens?

---

## TASK 2 — Model: bonding sDAI vs holding pDAI
**Priority: High — do after Task 1 once mechanism is confirmed**

### Variables to model once mechanism is known:
- Bond discount rate (e.g. 10% discount = you get $110 of pDAI for $100 of sDAI)
- Vesting period (e.g. 5 days, 30 days — during which pDAI price may move)
- DSR yield on sDAI during vesting (~5-6% APY, so ~0.07% per 5-day vest)
- Opportunity cost: sDAI sitting as collateral vs pDAI bought outright appreciating
- Break-even: at what bond discount does bonding beat just buying pDAI spot?

### Simple comparison framework:
```
Hold pDAI:        $100 → buy pDAI spot → if peg: $100 × 877 = $87,700
Bond sDAI:        $100 sDAI → receive $X pDAI at discount after Y days vesting
                  → if peg during/after vest: $X × 877 + DSR yield on $100 during vest
Bond wins if:     bond discount > 0% (any discount beats spot if peg timing is same)
Bond loses if:    pDAI price moves significantly during vesting period (you miss the move)
```

### Key risk to quantify:
- If pDAI pegs DURING the vesting period, bonded sDAI is still vesting at old discount
- You get pDAI delivered after peg — too late for the move
- Holding pDAI: you already have it when peg happens

---

## TASK 3 — Find psDAI contract address
**Priority: Medium**

### What to find:
- Is psDAI (forked sDAI / Savings DAI on PulseChain) a real token with a CA?
- ERC-4626 sDAI contract on Ethereum: `0x83F20F44975D03b1b09e64809B757c47f942BEeA`
- The forked version on PulseChain should be at same address — verify it exists and has liquidity
- If it exists: current price, market cap, any trading activity
- Is psDAI mentioned in the bonding mechanism?
- Any community discussion of psDAI specifically vs pDAI

### Where to search:
- PulseScan (scan.pulsechain.com) — look up `0x83F20F44975D03b1b09e64809B757c47f942BEeA` on PulseChain
- PulseCoinList — search "sDAI" or "Savings DAI"
- GoPulse — token search
- DexScreener PulseChain — any psDAI pairs?

---

## TASK 4 — Update docs once findings are in
**Files to update:**
- `STABLECONTEXT.md` — add §1.4 or update §5.5 with bonding mechanism details + sDAI/psDAI data
- `PDAI_DEEP_DIVE.md` — add new section on sDAI bonding math vs hold comparison
- `PDAI_CONSPIRACY.md` — update if bonding mechanism reveals new actor/wallet connections
- `PDAI_TIMELINE.md` — add bonding mechanism announcement event
- `MEMORY.md` + auto-memory — update with psDAI CA and bonding contract address

---

## QUICK REFERENCE FOR NEXT SESSION

**Known contract addresses:**
- pDAI (primary): `0x6b175474e89094c44da98b954eedeac495271d0f` (PulseChain)
- sDAI (Ethereum): `0x83F20F44975D03b1b09e64809B757c47f942BEeA`
- psDAI (PulseChain — unconfirmed): check same address on PulseChain
- HEX: `0x2b591e99afE9f32eAA6214f7B7629768c40Eeb39`

**Current state (Feb 2026):**
- pDAI system: ESM shutdown (`live = 0`) — frozen until reboot
- pDAI price: ~$0.00114, TVL $7.89M, vol $495K/day
- BetterBank: live on PulseChain (AAVE V3 fork, pDAI lending)
- RH SEC case: dismissed Feb 2025

**Open question driving all of this:**
> What exactly did RH say about bonding sDAI, and does the bonding contract exist yet?
