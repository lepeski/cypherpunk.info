# PDAI_CONSPIRACY.md
## Ranked Evidence: pDAI as a Coordinated Master Plan
**Compiled:** 2026-02-24
**Method:** Web search, on-chain forensics from community researchers, social media analysis
**Label convention:** `[VERIFIED]` = documented fact | `[ON-CHAIN]` = blockchain-traceable | `[COMMUNITY]` = unverified community claim | `[SPEC]` = speculation | `[UNVERIFIED]` = referenced but not independently confirmed

> **Scope note:** This document compiles conspiratorial, coincidental, and structurally suspicious evidence that pDAI's trajectory toward a $1 peg is coordinated rather than emergent. Evidence is ranked from most to least structurally significant. Verified facts, community beliefs, and speculation are explicitly labeled. This is not an endorsement of any theory.

---

## RANKED EVIDENCE LIST

---

### #1 — OA-CONNECTED WALLET MINTED pDAI **BEFORE** PULSECHAIN OPENED TO THE PUBLIC
`[ON-CHAIN]` `[VERIFIED]`

**What happened:**
On May 11, 2023 — two days before PulseChain launched to the public on May 13 — an Origin Address-connected wallet minted pDAI and performed MakerDAO vault operations on PulseChain before the chain was accessible to anyone else.

**Key detail:**
The same owner wallet controls PLS, PLSX, INC, MasterChef, and the **Eternal Storage Proxy for the entire PulseChain network** (address: `0x30e22ab6e6B576e6A9c5dD73191237a9A5c72539`). The MakerDAO PRC contracts were active and functional pre-launch.

**Why it's significant:**
Only a party with deep knowledge of — and access to — PulseChain's pre-launch infrastructure could have done this. The Eternal Storage Proxy controls upgradeable contract storage for the whole chain. Linking this to early pDAI minting implies the pDAI system was being tested or seeded by insiders before any public access.

**Source:** NineIronCapital thread / community on-chain research (threadreaderapp.com/thread/1692879099482800369.html)

---

### #2 — RICHARD HEART WALLET (2822) IS THE LARGEST pWBTC HOLDER AND RECEIVED 6.7 TRILLION PLSX AT LAUNCH
`[ON-CHAIN]` `[COMMUNITY]`

**What happened:**
Community researchers (NineIronCapital, DcentraliseMe) have identified wallet `0x3899e2b00fe4eda542021780039d69a583dd2822` (labeled "2822") as attributable to Richard Heart. This wallet is:
- The **largest pWBTC holder** on PulseChain
- Received **6.7 trillion PLSX** and **6.2 trillion PLS** at launch (Origin Address-tier distribution)
- Connected through forensic tracing to pMKR governance activity

**Why it's significant:**
If accurately attributed, this wallet has enormous latent collateral capacity. The pDAI governance proposal (Nov 2024) explicitly targets HEX/PLS/PLSX as pDAI collateral — assets this wallet holds in vast quantities. Governance + collateral control in one entity = capacity for unilateral peg.

**Caveat:** Wallet attribution to Heart is community inference, not documented proof. `[COMMUNITY]`

---

### #3 — THE GOVERNANCE CONTROL CHAIN: COORDINATED ATTACK DRAINING MAKERDAO ON PULSECHAIN (Jun–Jul 2023)
`[ON-CHAIN]` `[VERIFIED]`

**What happened:**
A sequence of precise, multi-step governance operations targeting pDAI's MakerDAO fork:

| Date | Wallet | Action |
|------|--------|--------|
| 28-Jun-23 | 9E6F (`0xa301...9e6f`) | Purchased 320.5k pAAVE to initiate governance vote |
| 28-Jun-23 | 9E6F | Withdrew 1.26M pAAVE from staked vaults |
| ~Jul-23 | 9E6F | Drained 58k pMKR from AAVE interest-bearing Maker vault |
| 3-Jul-23 | 9E6F | Extracted pLINK, YFI, pUNI, pWBTC worth ~566 ETH → **Tornado Cash** |
| 8-Jul-23 | B22F (`0x2082...b22f`) | Received pMKR vaults with 11,941.91 pWBTC (~$1.1M) |
| 8-Jul-23 | B22F | Converted to ETH → **547 ETH via Tornado Cash** |
| ~Jul-23 | 9E6F | Sent 46.2k pMKR to 3F9D wallet → **paused all governance** |
| Post-Jul | 17F7 (`0xa618...17f7`) | Received pMKR governance rights; performed testnet recapitalization and MKR token burning experiments |

**Why it's significant:**
This is not opportunistic arbitrage — it's a sequential governance acquisition operation. The drain liquidated competing governance stake, routed funds through Tornado Cash (destroying forensic trail), and transferred governance control to a new wallet. Community researchers attribute the 9E6F→17F7 chain to RH based on cross-reference with wallet 2822.

**Source:** pulsechaindai.com/research/ (NineIronCapital forensics)

---

### #4 — LIDO DAO REPLACED MKR ON PULSECHAIN PRE-LAUNCH VIA ARAGON CO-FOUNDER WALLET
`[ON-CHAIN]` `[COMMUNITY]`

**What happened:**
`dev.izqui.eth` — wallet of Jordi Baylina, co-founder of **Aragon** (the governance framework used by **Lido DAO**) — was identified as the **contract creator** for pDAI wallet infrastructure on PulseChain. This activity occurred **the day before PulseChain launched**.

**NineIronCapital claim:** "LIDO DAO replaced MKR on PulseChain pre-launch. The wallet dev.izqui.eth was the contract creator, and izqui is the co-founder of Aragon, the governance framework DAO that Lido uses."

Additional claim: stETH minting operations were linked to both PulseX LP positions and Atropa-USDC operations, suggesting cross-chain capital coordination involving Lido's liquid staking infrastructure.

**Why it's significant:**
If accurate, this connects pDAI's infrastructure to one of Ethereum's largest liquid staking protocols (Lido, ~$20B TVL) before PulseChain even launched. Two feeder wallets (`0x80eb...5AB` and `0x886e...8c2`) allegedly created a "confusing circular loop" in early on-chain operations.

**Caveat:** The full izqui9/Lido claim is community-level research and has not been independently verified by third-party blockchain analytics firms. `[COMMUNITY]`

---

### #5 — cUSDCv3 PROPOSAL ON ARBITRUM FILED **TWO DAYS BEFORE** PULSECHAIN LAUNCH
`[ON-CHAIN]` `[VERIFIED]`

**What happened:**
NineIronCapital found a **Compound governance proposal to install cUSDCv3 on Arbitrum**, dated **May 8, 2023** — exactly two days before PulseChain's launch. Multiple confirmed "pDAI pioneer wallets" interact with this same cUSDCv3 contract.

**The coincidence:**
- Compound cUSDCv3 proposal: May 8, 2023
- "Airdrop wallet" 86FF created: May 11, 2023
- PulseChain launch: May 13, 2023
- Three related events within a 5-day window

**Additional detail:**
Wallet "5996" later took over Arbitrum L2 and upgraded it. Pre-5996 smart contracts were found that "code exactly for what to do within the Maker vault **should the ESM happen**" — meaning someone pre-coded MakerDAO emergency shutdown handling before PulseChain launched.

**Why it's significant:**
Pioneer wallets linked to pDAI's early activity were simultaneously active in Compound governance on Arbitrum during PulseChain's launch window. The pre-coded ESM handling implies foreknowledge of a shutdown scenario years before one occurred.

**Source:** DuRtY Crypto / NineIronCapital (x.com/DuRtY_Crypto/status/1976268406480359434)

---

### #6 — RICHARD HEART TWEETED ABOUT THE ESM "FIRE FUNCTION" WITH INSIDER-LEVEL TECHNICAL PRECISION
`[VERIFIED]`

**What happened:**
On approximately April 17, 2025, Richard Heart tweeted:
> *"The pDAI cancer may be coming to an end. 22 hours ago someone ran the fire function on the ESM module, which runs the cage function in the end contract, which begins the shut down of the system. The system is in shutdown mode as evidenced by 'live' having a 'o' for status."*
— @RichardHeartWin (x.com/RichardHeartWin/status/1912747524248748185)

**Why it's significant:**
- The ESM (Emergency Shutdown Module) is a highly technical, rarely-discussed component of MakerDAO architecture
- Heart described the internal state variable (`live = 0`) and the exact function call chain (`fire() → cage()`) with precision that surprised observers
- He framed the shutdown as the end of "cancer" — implying knowledge of or desire for this outcome
- The price subsequently crashed 99.99% (from ~$0.034 to $0.000002)
- `[SPEC]` Community theory: RH knew the fire function would be called, or called it himself, as a reset mechanism before a controlled peg event

---

### #7 — PULSEMAKER GOVERNANCE PROPOSAL: RH'S OWN TOKENS AS pDAI COLLATERAL (Nov 2024)
`[VERIFIED]`

**What happened:**
On November 21, 2024, community members **DcentraliseMe, NineIronCapital, Konenstein, and Freedom_777** filed a formal PulseMaker governance proposal to add HEX, PLS, and PLSX as pDAI collateral types.

**Parameters proposed:**
- Collateralization ratio: **110%** (extremely low for DeFi standards; typical is 150%+)
- Liquidation ratio: **10%**
- Stability fee: **0%**
- Initial debt ceiling: **0** (with review planned)
- Explicit goal: "Enable the Origin Address (OA) to back the existing pDAI supply"

**Peculiar detail:**
The official GitHub proposal (PulseMakerWin repository) references **"Richard Heart regarding confidentiality agreements"** — explicitly naming Heart in the governance documentation of a project he publicly distances himself from.

**Why it's significant:**
If the OA's HEX/PLS/PLSX holdings back pDAI at 110% collateralization, the OA effectively controls the peg. The entire pDAI supply could theoretically be collateralized by assets the Origin Address already holds — requiring no external capital.

**Source:** raw.githubusercontent.com/PulseMakerWin/community/master/governance/polls/Proposal%20to%20add%20core%20PulseChain%20coins%20as%20collateral.md

---

### #8 — pCOMP TIMELOCK TAKEOVER: OFFICIAL AIRDROP WALLET CONTROLS COMPOUND ON PULSECHAIN
`[ON-CHAIN]` `[COMMUNITY]`

**What happened:**
A mysterious entity executed a **Timelock transaction** to take over the pCOMP (Compound) admin function on PulseChain, finalizing control of the **cDAI contract** (Compound's DAI lending market).

**Key detail:**
The sender wallet is identified as the **official PulseChain Airdrop wallet**, connected to an **AMM Fixer Bot**.

**NineIronCapital/DuRtY Crypto quote:**
> *"Someone is officially about to take over Compound on our L1. When you see who's behind it, your mind will be blown."*
— DuRtY Crypto (x.com/DuRtY_Crypto/status/2008469946142192096)

**Why it's significant:**
Control of Compound's cDAI contract on PulseChain means controlling the primary **lending market for pDAI** — where users borrow and deposit pDAI. Whoever controls cDAI controls borrowing rates, liquidation thresholds, and collateral acceptance. Linking this to PulseChain's own official Airdrop wallet is structurally explosive if confirmed.

---

### #9 — THE PSM EXPLOIT: $3.62M EXTRACTED, BUT WAS IT A FEATURE?
`[ON-CHAIN]` `[VERIFIED]`

**What happened:**
From January 26, 2025 onward, 4 wallets minted **683,842,309.60 pDAI** using the DssPsm `sellGem()` function, extracting **$3,623,261.89** from the PulseChain ecosystem. The mechanism:
1. Exchange PLS → pUSDC
2. Call `sellGem()` on DssPsm → convert pUSDC 1:1 into newly minted pDAI
3. Sell minted pDAI for PLS (when pDAI trades at premium vs pUSDC)
4. Repeat

**The wrinkle:**
This is not a traditional hack. The PSM (Peg Stability Module) is an **intentional MakerDAO design feature** meant to maintain the peg by allowing 1:1 USDC→DAI conversion. On PulseChain, pUSDC trades far below $1, making this an "exploit" only because of market conditions.

**Community theory (`[SPEC]`):**
The PSM exploit inflated pDAI supply from ~10B to 44B+, making pDAI look "worthless" by market cap dilution — but this also distributed pDAI widely across wallets, potentially setting up a massive redistribution gain if peg is achieved. Some theorists argue this was a **deliberate supply inflation phase** to lower the per-token price before a peg event multiplies everyone's holdings.

**Source:** HashMiner analysis (@Hash_Miner/status/1903201916147896751); RH tweets on exploit

---

### #10 — RICHARD HEART TWEETED "REMOVE ALL LIQUIDITY FOR pDAI" WHILE SUPPLY GREW 213M DURING HIS TWEETS
`[VERIFIED]`

**The paradox:**
Richard Heart tweeted that "life would be better if everyone removed all liquidity for pDAI vs everything else" — yet the pDAI supply grew by **213,546,101** *during the period he was tweeting about exploiters*.

He also tweeted:
> *"Something has inflated the pDAI supply by multiples... pDAI has 24.5B supply now. DAI had under 10B at the Ethereum fork. Who's minting that supply and why?"*

**Two interpretations:**
1. **Standard:** Heart is warning the community about real exploiters he cannot stop
2. **`[SPEC]` Conspiracy:** The supply inflation was controlled; Heart's tweets directed retail to remove LP, which reduced liquidity depth and would magnify price impact when a future peg event occurs (less TVL = easier to peg)

---

### #11 — GOVERNANCE PAUSE VIA 46.2k pMKR TO 3F9D WALLET: ALL VOTES HALTED
`[ON-CHAIN]`

**What happened:**
The 9E6F wallet sent **46,200 pMKR** into MakerDAO's governance pause contract (`0x3dc4d01d683f30e1ca6e0faffbef0276a31a3f9d` / 3F9D), halting **all governance votes** on PulseChain's MakerDAO fork for an extended period.

After the pause, the 9E6F wallet set the governance owner to the **B22F wallet**, which then drained pMKR vaults.

**Why it's significant:**
Pausing governance freezes any community attempt to intervene in the system. This happened concurrently with the asset drain in Jul 2023. A hostile actor would pause governance to prevent community defense; a controlled actor would pause it to prevent interference with a planned sequence.

---

### #12 — CATTIE (XUSD TEAM) TAKES OVER pDAI MAKERDAO GOVERNANCE POST-EXPLOIT
`[COMMUNITY]`

**What happened:**
After the 2023 governance attack, a figure named **Cattie**, described as a member of the **XUSD team** (another PulseChain stablecoin project), took over governance of pDAI's MakerDAO fork on PulseChain.

**Why it's weird:**
A competing stablecoin team controlling the governance of pDAI creates a significant conflict of interest — and raises the question of whether XUSD and pDAI are actually competing, or whether they serve different roles in a coordinated PulseChain stablecoin stack.

**Note:** "Casssy" referenced by the user was not independently found in searches — Cattie is the closest confirmed figure in this governance narrative. `[UNVERIFIED for Casssy specifically]`

---

### #13 — MARIA RAHEL DUMP: ATROPA DEVELOPER SELLS pDAI → TRIGGERS 69% COLLAPSE AND ATROPA CASCADE
`[COMMUNITY]`

**What happened:**
In mid-March 2025, a developer referred to as **"Maria"** (allegedly Maria Rahel, tied to the Atropa ecosystem) reportedly sold large bags of pDAI for ETH, triggering a **69% price collapse** in pDAI. This cascaded into the Atropa and BEAR token liquidity pools, causing significant collateral damage.

**Why it's suspicious:**
- Atropa was positioned as pDAI's liquidity backbone (see §5.2 of STABLECONTEXT)
- A key Atropa developer exiting pDAI positions mid-strategy would be either:
  - A betrayal of the plan (`[SPEC]` "Cryptosolv dump" theory), OR
  - A coordinated shakeout to reset the entry point at a lower price
- Atropa's burned liquidity pools persisted after the dump — the "floor" mechanism survived

---

### #14 — SOMMI WORE pDAI LOGO NECKLACE AT HEX CONFERENCE → pDAI PUMPED 20%
`[VERIFIED]`

**What happened:**
At the **6th Annual HEX Conference**, influencer **@yourfriendSOMMI** was observed wearing a **pDAI logo necklace**. The community immediately noted this, and pDAI pumped **+20%** in response.

**Context:**
Sommi has been described by community members as having "hit every meta on PulseChain" — being early on HEX narratives, then PulseChain/PLSX, and now pDAI. Community observers note the pattern with suspicion:

> *"Our friend Sommi has hit every meta on PulseChain 🔥 First, TangGang tickers like HOA and DWB, then PokeChain like PIKA and CHARM, and now the big pegging of pDAI."*
— @MoJuiceX

**`[SPEC]`:** Either Sommi has extraordinary on-chain intuition, or there is coordination between the pDAI narrative team and high-profile community influencers.

**Source:** x.com/yourfriendSOMMI/status/2008742493815451983

---

### #15 — BETTERBANK (AAVE V3 FORK): pDAI GETS LENDING UTILITY AFTER 2+ YEARS, BUILT IN PARALLEL
`[VERIFIED]`

**What happened:**
**BetterBank** — a modified Aave V3 fork — launched on PulseChain, providing pDAI with its **first-ever lending utility**. The team reportedly took **more than a year** to build it. Features:
- Users deposit pDAI, borrow against it, use proceeds to buy more pDAI → **leverage loop**
- Stronghold: high-yield savings for PLS, PLSX, and pDAI (50–72% APY claimed)
- Wildlands: LP-backed credit facility
- Also planned for Arbitrum deployment

**Why it's suspicious:**
BetterBank was built quietly over 1+ year while pDAI was trading at near-zero. A lending protocol purpose-built around pDAI implies builders expected pDAI to be worth enough to loop — suggesting either irrational faith or foreknowledge of a peg event.

The loop mechanism is functionally similar to **Anchor Protocol's 20% APY** on UST — reflexive demand that accelerates price. The question is whether this is coincidental design convergence or deliberate.

**Source:** DuRtY Crypto (x.com/DuRtY_Crypto/status/1951623843350814743); Medium post by @betterbankbb

---

### #16 — THE PSM "EXPLOIT" WALLETS: POSSIBLE CONTROLLED SUPPLY INFLATION THESIS
`[SPEC]` `[ON-CHAIN]`

**Background:**
The 4 PSM arbitrage wallets extracted $3.62M while inflating pDAI supply by ~680M tokens. All extracted value was "completely bridged out of the chain without flowing back."

**Community thesis (NineIronCapital):**
These wallets may not be random arbitrageurs. The PSM arbitrage requires:
1. Understanding of DssPsm mechanics (DeFi-literate actors)
2. Access to significant pUSDC liquidity
3. Sustained operation over weeks without being stopped

If the pDAI system's controllers knew about the PSM vulnerability but did not disable it, the inflation could be intentional — building a large circulating supply at low prices, then triggering ESM to reset the system, then relaunching with a new peg mechanism backed by OA collateral.

**Counterargument:** The PSM exploit was disabled only after the ESM fire function was called — consistent with either interpretation.

**Note on "p dong exploiter":** This nickname was referenced by the user but was not found in web searches. It may be a community nickname for one of the 4 PSM arbitrage wallets. `[UNVERIFIED]`

---

### #17 — THE "CONSPIRACY PEG PROPHECY" NARRATIVE ITSELF: COMMUNITY SELF-FULFILLMENT
`[SPEC]`

**The meta-observation:**
The belief that pDAI will peg to $1 is itself a market force. Community accounts (@TheGreekGod11, @files_dirty, @liquidsoil369, @NineIronCapital, @yourfriendSOMMI) have built a narrative ecosystem around "pDAI is destined to peg." This narrative:
- Creates buying pressure at depressed prices
- Attracts capital anticipating the "peg event"
- Generates social proof (necklaces, conferences, threads)
- Provides cover for large-wallet accumulation ("if I know it's going to peg, I accumulate when others are scared")

**Whether or not the plan is coordinated, the narrative is doing the work of coordination.**

---

### #18 — BINANCE OFFICIAL ACCOUNT POSTS: HEART EMOJI + LIGHTSABER — COMMUNITY READS AS RH SIGNALS
`[USER-CONFIRMED]` `[CONTENT UNVERIFIABLE VIA SCRAPE]`

Both posts confirmed real by user. X blocks all automated fetching so visual content cannot be extracted, but URLs are live.

**Post 1 — The Heart Post**
- URL: x.com/binance/status/1864264858989920287
- Estimated date: **~Dec 2024** (based on Snowflake ID position relative to other dated tweets)
- Community interpretation: Binance's official account posted content featuring a ❤️ / heart reference — read by pDAI community as a symbolic nod to **Richard Heart**, whether intentional or not
- Alternative reading: Routine Binance marketing content (holiday, campaign, etc.) with no PulseChain intent

**Post 2 — The Lightsaber Post**
- URL: x.com/binance/status/1918908612535083465
- Estimated date: **~May 4, 2025** (Star Wars Day — "May the 4th be with you" is a common brand post date)
- Community interpretation: The lightsaber image allegedly resembles the **PulseX logo** (which is stylized as a cross/plus mark that community members read as a blade shape) — interpreted as Binance subtly referencing or endorsing PulseX
- Alternative reading: Standard Star Wars Day marketing; PulseX logo similarity is coincidental pareidolia

**Why the community finds this significant:**
Binance is the world's largest crypto exchange. Any visual or symbolic overlap with Richard Heart's ecosystem — even if accidental — would represent extraordinary implicit validation for an asset trading at 877× below its target peg. The timing of the heart post (~Dec 2024, during the period when the OA collateral governance proposal was active) adds to the suspicion.

**Verdict:** Both posts exist and are confirmed. Whether the content constitutes meaningful coincidence requires viewing the actual images — check the URLs directly on X.

---

### #19 — RICHARD HEART "MakerDAO, DO THE FUNNIEST THING" TWEET
`[VERIFIED]`

**What happened:**
Prior to the ESM event, Richard Heart publicly tweeted at MakerDAO encouraging them to "do the funniest thing" — a phrase interpreted by the community and Protos as **Heart encouraging MakerDAO to execute a rug pull or emergency shutdown of pDAI**.

He framed this as calling their bluff, but the community read it as Heart signaling his awareness that a shutdown was coming — or his desire for one, as a reset mechanism.

**Source:** protos.com/richard-heart-pokes-makerdao-to-do-the-funniest-thing-and-rug-pull/

---

### #20 — AIRDROP WALLET CREATED MAY 11, pDAI MINTED MAY 11, CHAIN LAUNCHED MAY 13
`[ON-CHAIN]` `[VERIFIED]`

**The 5-day cluster:**

| Date | Event |
|------|-------|
| May 8, 2023 | Compound cUSDCv3 governance proposal filed on Arbitrum |
| May 11, 2023 | PulseChain "86FF" Airdrop Wallet created |
| May 11, 2023 | OA-connected wallet mints pDAI pre-launch |
| May 11, 2023 | MakerDAO PRC contracts tested on chain |
| May 13, 2023 | PulseChain launches publicly |

Five significant, apparently coordinated events in a 5-day window straddling launch day. The Compound/Arbitrum proposal connecting the same pioneer wallets creates a cross-chain coordination signal that is difficult to explain as coincidence.

---

## SUMMARY ASSESSMENT

### The Core Question:
Is pDAI's journey toward $1 an emergent community phenomenon, or a pre-architected event being executed in stages?

### Evidence That Suggests Coordination:
1. Pre-launch pDAI minting by OA-connected wallet with chain-level admin access
2. The 2023 governance drain (9E6F→B22F→17F7) was multi-step, precise, and routed through Tornado Cash — not casual arbitrage
3. Governance proposal explicitly names RH and proposes his assets as pDAI collateral
4. cUSDCv3 Arbitrum timing + pioneer wallet overlap is statistically improbable as coincidence
5. Lido/izqui9 infrastructure creation the day before launch
6. ESM "fire function" tweet shows insider-level MakerDAO knowledge from a man who publicly claims distance from pDAI
7. BetterBank built over 1+ year in anticipation of pDAI having value
8. Compound takeover via official Airdrop wallet — control of lending infrastructure

### Evidence Against Coordination (or for Chaos):
1. No hard wallet proof linking RH directly to 9E6F or B22F
2. Richard Heart has publicly and repeatedly distanced himself from pDAI
3. Maria Rahel dump (if real) would be irrational for a coordinator to permit
4. PSM exploit ran for weeks — a controller would shut it down faster
5. pDAI has been at near-zero for 2+ years with no peg — patience would be unusual
6. Binance posts not independently verifiable

### Verdict (Neutral):
The structural evidence is **more consistent with loose coordination by multiple sophisticated actors who share aligned incentives** (RH ecosystem, Lido/Compound power users, Atropa developers) than with either:
- Pure coincidence (too many precise timings), or
- A single mastermind controlling every variable (the Maria dump and PSM exploit duration argue against tight control)

The most parsimonious model: a small group of DeFi-native actors with insider knowledge of PulseChain's launch structure positioned early, have been managing governance levers since mid-2023, and are now (2025–2026) activating the peg infrastructure they pre-built.

---

## KEY ACTORS SUMMARY

| Actor | Role | Status |
|-------|------|--------|
| Richard Heart | PulseChain founder, publicly distant from pDAI, ESM tweet suggests proximity | Public figure |
| NineIronCapital | Primary on-chain researcher, authored conspiracy threads and governance proposals | Pseudonymous |
| DcentraliseMe | Co-authored Nov 2024 governance proposal | Pseudonymous |
| DuRtY Crypto | Amplifies NineIronCapital research; Compound takeover thread | Pseudonymous |
| yourfriendSOMMI | Influencer, pDAI necklace at HEX Conference | Semi-public |
| Cattie (XUSD team) | Took over MakerDAO governance post-exploit | Pseudonymous |
| Maria Rahel | Alleged Atropa developer who dumped pDAI Mar 2025 | Semi-public |
| dev.izqui.eth (izqui9) | Aragon co-founder, alleged pDAI infrastructure creator | Public (Jordi Baylina) |
| 9E6F wallet | Governance drain executor (Jun–Jul 2023) | Unknown |
| B22F wallet | Funds recipient, Tornado Cash | Unknown |
| 17F7 wallet | Post-drain governance controller | Unknown |
| 2822 wallet | Alleged RH wallet, largest pWBTC holder | Alleged = RH |
| "Casssy" | User-referenced figure; not independently found | `[UNVERIFIED]` |
| "p dong exploiter" | User-referenced nickname for PSM arbitrageur(s) | `[UNVERIFIED]` |

---

## ACCOUNTS TO FOLLOW FOR ONGOING RESEARCH

- **@NineIronCapital** — primary on-chain forensics, governance threads
- **@DuRtY_Crypto** — amplification and synthesis of NineIronCapital findings
- **@yourfriendSOMMI** — community narrative and influencer signals
- **@TheGreekGod11** — user-cited; unverified content (check directly on X)
- **@files_dirty** — user-cited; unverified content (check directly on X)
- **@liquidsoil369** — user-cited; unverified content (check directly on X)
- **@pulsedai** — official pDAI community account

---

*For LP/peg scenario modeling see PDAI_DEEP_DIVE.md. For full ecosystem background see STABLECONTEXT.md.*
