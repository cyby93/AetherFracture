# Aether Fracture — Prototype Reference

## 1. Setup

### Map construction

- **Center:** The Shard (1 hex)
- **Rings:** Build outward based on player count
	- 2 players: Center + Ring 1 + Ring 2 — 19 hexes total
	- 3 players: Center + R1 + R2 + half of R3 — ~28 hexes
	- 4 players: Center + R1 + R2 + R3 — 37 hexes
- **Tile draft:** Randomly draw tiles to fill the rings (recommended split: 30% plains, 20% defensive, 15% obstacles, 25% resources)

### Player start

- **Starting city:** Place 1 starting city on the edge of the outermost ring
- **Units:** Place 1 Hero and 2 Tier 1 Infantry on your city
- **Resources:** Set trackers to 4 Iron, 0 Aether, 3 Command
- **Deck:** Shuffle your 10-card starting deck and draw 5 cards

## 2. Turn structure

The game is played in rounds. A round ends when all players pass.

### Phase A — Production (start of round)

- **Reset:** Iron resets to 0 (except for factions that modify this). Command resets to current cap (default: 3)
- **Income:** Gain Iron and/or Aether from controlled quarries/mines/veins and from card effects
- **Draw:** Ensure you have 5 cards in hand

### Phase B — Action phase (player turns)

On your turn, spend Command points to perform actions; 1 Command = 1 card play.

- **Play a card:** Resolve either the top (combat/move) or bottom (economy) effect as printed
- **Move:** Move units according to the card effect (e.g., "Move 2 units up to 2 hexes")
- **Recruit:** Spend Iron to place units at your city (recruiting does not cost Command)
	- Tier 1: 2 Iron
	- Tier 2: 5 Iron + 1 Aether
	- Tier 3: 10 Iron + 3 Aether (Epoch II+ only)
- **Market:** Buy a card from the market row (pay the Iron cost and place the purchased card into discard)

### Phase C — Cleanup

- Discard played cards
- Keep any unspent Aether
- Iron resets to 0

## 3. Combat rules

Combat occurs when a unit moves into an enemy-occupied hex.

### The combat sequence

1. **Declare attack:** Attacker moves into the hex
2. **Commit cards (The Bluff):** Both players choose 1 card from hand and play it face-down
3. **Reveal & calculate:**

	 Total Strength = Unit base strength + Card bonus + Terrain bonus

4. **Resolution:**

	 - Defender wins (Def > Att): Attacker retreats to the previous hex. No casualties.
	 - Attacker wins (Att > Def): Defender retreats 1 hex.
	 - Damage: If the defender is a T2 or T3 unit, it loses 1 HP; T1 units are only pushed and take no HP.
	 - Overkill (Att ≥ Def × 2): Defender is destroyed instantly (removed from the board)

### Unit stats

- **Tier 1 (Infantry):** 2 Str / 1 HP / Move 2
- **Tier 2 (Specialist):** 5 Str / 2 HP / Move 2
- **Tier 3 (Titan):** 9 Str / 4 HP / Move 1

## 4. Terrain & tile effects

- **Plains:** Standard movement, no bonuses
- **Forest / Ruins (defensive):** +1 combat strength to the defender
- **Mountain / Deep water (obstacle):** Cannot be entered by T1/T2 units (unless a specific "Climb/Swim" tech or card is used)
- **Iron quarry:** Controller gains +1 Iron per turn
- **Aether vein:** Controller gains +1 Aether per turn
- **The Shard (center):** Grants +1 Command per turn to its controller

## 5. The Epoch system (game timer)

- **Epoch I (Rounds 1–4):** Standard play
- **Epoch II (Rounds 5–8):** Tier 3 Titans unlock; "Volatility" events begin
- **Epoch III (Rounds 9–12):** The Void

Important round effects:

- **Round 9 end:** Remove the outermost ring (units in that ring are destroyed)
- **Round 10 end:** Outer ring takes ongoing Void damage
- **Round 12:** Game ends — highest score wins (territory + Aether + tech)