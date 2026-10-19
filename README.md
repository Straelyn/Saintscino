# Lucky Hangar — Smart Storage Unit slot machine for EVE Frontier

A slot machine that runs on a **Smart Storage Unit** in EVE Frontier (Stillness).
Bet building materials, win **SOF-40** and **EU-40 Fuel**. Every spin is a transaction on the
Sui blockchain, so the odds are enforced by the contract, not by the website.

**Play / dApp:** https://straelyn.github.io/Saintscino/

---

## How to play

1. Fly to a storage unit running the casino and open its dApp window.
2. **Connect EVE Wallet** (top right).
3. Drag your stake into **your own slot** in the unit (the STORAGE UNIT panel).
   Accepted: **Thermal Composites**, **Carbon Weave**, **Reinforced Alloys**.
   The page shows what's in your slot.
4. Pick the material and a bet size (**1**, **5** or **10**), then press **Pull** and approve in your wallet.
5. Pushes and winnings land in your slot. Drag them out whenever you like.

Each spin costs a tiny amount of SUI for gas (about 0.001 SUI).

## Payouts (standard table)

Three of a kind pays:

| Symbols | Result | Chance | Pays |
|---|---|---|---|
| Rift - Wild ×3 | 50x | 0.2% | SOF-40 Fuel |
| EVE Core ×3 | 40x | 0.5% | SOF-40 Fuel |
| LUX Split ×3 | 30x | 1.5% | SOF-40 Fuel |
| Asteroid ×3 | 20x | 5% | EU-40 Fuel |
| Feral Bar ×3 | Push | 15% | your stake back |
| anything else | Lose | 77.8% | — |

Example: a 20x win on a 1-unit bet pays 20 fuel; on a 10-unit bet, 200.
Each casino's owner can choose SOF-40 or EU-40 per win tier, so check the
**Three of a kind pays** list on the page for the casino you're at.

## Is it fair?

- The result comes from Sui's on-chain random number generator, inside the contract.
  The website only shows the result; it can't pick or change it.
- The contract can't be called in a way that lets anyone "roll, look, and cancel if they lose".
- If the house can't cover a win, the spin is cancelled and you keep your stake.

## Run a casino on your own storage unit

1. Set your unit's dApp URL to `https://straelyn.github.io/Saintscino/?setup=1`
   (players never see the owner panel, so you can leave `?setup=1` on).
2. Open the dApp at your unit, connect your EVE wallet, press **Set up a casino on this unit**.
   This creates your own casino (you're its admin) and installs the slots extension
   (it replaces any other extension on the unit).
3. Stock the prizes in the unit's **main inventory**: at least **500 SOF-40** and **200 EU-40**
   covers the biggest wins on 10-unit bets (the panel recalculates if you change payouts).
4. Choose SOF-40 / EU-40 per tier under **Payouts**, then press **Open casino**.

Notes for owners:
- You can't play at your own unit: your drag-ins go to the bankroll, not a personal slot.
- Stakes collect in the unit's main inventory. Move them out now and then to keep space free.
- If a unit changes hands, the new owner presses **Claim this casino** to take over.


Questions, revisions or contract updates: **Straelyn - message in game**.
