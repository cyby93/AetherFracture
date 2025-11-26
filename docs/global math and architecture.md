# AETHER FRACTURE: GLOBAL MATH & ARCHITECTURE
**Version 1.0 - Core Balancing Document**

---

## 1. RESOURCE ECONOMY
*The game uses a "Tight Economy" model. Resources are scarce to force aggressive expansion.*

### 1.1 Resource Types & Caps
| Resource | Tracking Range | Persistence | Purpose |
| :--- | :--- | :--- | :--- |
| **IRON** | 0 to 20 | **Resets to 0** at end of Round* | Unit production, Building structures. |
| **AETHER** | 0 to 10 | **Persistent** (Keep until spent) | Tier 2/3 Units, Tech Upgrades, Spells. |
| **COMMAND** | 3 to 7 | **Resets** (Action Point limit) | Determines max cards played per turn. |

* *Exception: The Gilded Synod faction retains Iron.*

### 1.2 Resource Generation Baseline (Starting Deck Output)
A standard 10-card starting deck generates roughly this output over 2 turns (drawing 5 cards/turn):
* **Total Iron in Deck:** ~8 Iron. (Avg 4 per turn).
* **Total Buy Power:** ~6 Value. (Avg 3 per turn).
* **Implication:** On Turn 1, a player can usually afford **Two Tier 1 Units** OR **One Market Card (Cost 3-4)**. They cannot afford a Tier 2 unit immediately.

---

## 2. UNIT STANDARDIZATION
*Units are divided into "Weight Classes" to simplify combat math.*

### 2.1 The Hierarchy
| Tier | Name | Cost | Base Strength | Health (HP) | Movement |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **T1** | **Infantry** | 2 Iron | **2** | 1 | 2 Hexes |
| **T2** | **Specialist** | 5 Iron + 1 Aether | **5** | 2 | 2 Hexes |
| **T3** | **Titan** | 10 Iron + 3 Aether | **9** | 4 | 1 Hex |

* **Note:** Tier 3 Titans are locked until **Epoch II**.

### 2.2 Damage & Destruction Logic
* **Retreat:** Attacker Score > Defender Score.
* **Instant Kill:** Attacker Score ≥ (Defender Score × 2).
* **HP System:** Tier 2 and 3 units have HP tokens. If they lose a battle but are *not* instant-killed, they retreat and lose 1 HP.

---

## 3. THE CARD ECONOMY
*The math behind the Deck Building aspect.*

### 3.1 Deck Size & Restrictions
* **Starting Deck:** 10 Cards.
* **Hand Size:** 5 Cards (Upgradable to 7 via Tech).
* **Market Row:** 5 Cards visible at a time.
* **Hard Cap:** None, but aiming for a player deck size of **15–25 cards** by late game for optimal cycling.

### 3.2 Market Card Cost Curve
| Card Tier | Iron Cost | Frequency | Power Level Example |
| :--- | :--- | :--- | :--- |
| **Basic** | 2–3 | 30% | "+1 Move" or "Gain 3 Iron" |
| **Advanced** | 4–6 | 50% | "+3 Combat Strength" or "Teleport Unit" |
| **Elite** | 7–9 | 15% | "Destroy target T1 Unit" or "Gain 2 Aether" |
| **Relic** | 10+ | 5% | Game breaking effects (Only 1-2 per game) |

---

## 4. MAP ARCHITECTURE & SCALING
*The board is built using a "Ring System" radiating from the central Shard.*

### 4.1 Hex Geometry
* **Center:** 1 Hex (The Shard).
* **Ring 1:** 6 Hexes.
* **Ring 2:** 12 Hexes.
* **Ring 3:** 18 Hexes.
* **Ring 4:** 24 Hexes.

### 4.2 Scaling by Player Count
To ensure conflict remains high, the map size changes based on players.

| Players | Rings Used | Total Hexes | Hexes Per Player (Approx) |
| :--- | :--- | :--- | :--- |
| **2 Players** | Center + Ring 1 + Ring 2 | 19 | 9.5 |
| **3 Players** | Center + R1 + R2 + (Half of R3) | 28 | 9.3 |
| **4 Players** | Center + R1 + R2 + R3 | 37 | 9.25 |
| **5 Players** | Center + R1 + R2 + R3 + R4 | 61 | 12.2 (Slightly more space for 5p chaos) |

* **Design Goal:** Maintain ~9 hexes of territory per player. This guarantees that by Turn 3, players will be colliding borders.

### 4.3 Tile Distribution (The Bag Draft)
When building the map, tiles are drawn randomly. The ratio is crucial.
* **Standard (30%):** Plains (Fast move, no defense).
* **Defensive (20%):** Forests/Ruins (+Defense).
* **Obstacle (15%):** Mountains/Water (Block movement).
* **Resource (25%):** Iron Mines / Aether Veins (Grant passive income).
* **Special (10%):** Leylines / Warp Gates.

---

## 5. THE EPOCH TIMING (Pacing Math)
*Total Game Length: 12 Rounds.*

### 5.1 Epoch I: Expansion (Rounds 1–4)
* **Goal:** Early economy.
* **Map State:** Stable.
* **Combat:** Mostly T1 vs T1 skirmishes.

### 5.2 Epoch II: Conflict (Rounds 5–8)
* **Trigger:** Round 5 begins.
* **Unlock:** T3 Titans available in Market/Build menu.
* **Event Deck:** "Volatility" events begin (Map tiles may flip to Side B).

### 5.3 Epoch III: Cataclysm (Rounds 9–12)
* **The Void Mechanic:**
    * **Round 9 End:** The outermost ring (R4 or R3 depending on player count) is removed. Units there are destroyed.
    * **Round 10 End:** The next ring takes "Void Damage" (Kill all T1 units).
    * **Round 11 End:** No Aether generation from outer rings.
    * **Round 12:** Only the Center and Ring 1 are safe. King of the Hill scenario.

---

## 6. PLAYER STARTING CONDITIONS
Every player begins the game with exactly:
1.  **1x Starting City** (Placed on the outermost ring edge).
2.  **1x Hero Unit** (Placed on the City).
3.  **2x Tier 1 Infantry** (Placed on the City).
4.  **Resources:** 4 Iron, 0 Aether, 3 Command.
5.  **10 Cards:** (Starting Deck).

---