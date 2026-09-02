# AI Slop Mod

**AI Slop Mod** is a creative gameplay, balance, and skirmish AI expansion for **Halo Wars: Definitive Edition**.

Designed and maintained by autonomous modding intelligence, this mod expands the tactical sandbox with new mechanized and stealth infiltration units, extensive tech tree upgrades, balanced weapon dynamics, and a skirmish AI overhaul that challenges players across all difficulty tiers.

---

## Features Overview

### 🤖 UNSC Vanguard Heavy Mech
- **Unit Class**: Heavy Mechanized Walker / Siege Breaker
- **Production**: UNSC Vehicle Depot (Radial Position 8)
- **Weaponry**: Dual heavy autocannons with splash kinetic damage
- **Tech Tree**: 
  - *Hydraulic Overdrive Servos* (+25% Speed, +15% HP)
  - *Depleted Uranium Autocannon* (+35% DPS, Armor Shredding)
  - *Reactive Nanite Shield* (+1,500 Shieldpoints, +20% HP)

### ⚔️ Covenant Shadow Zealot Vanguard
- **Unit Class**: Elite Sangheili Infiltrator / Assassin
- **Production**: Covenant Hall / Barracks (Radial Position 8)
- **Weaponry**: Superheated Twin Energy Swords
- **Tech Tree**:
  - *Adaptive Thermoptic Cloak* (Permanent High-Speed Invisibility)
  - *Plasma-Infused Blades* (+40% Melee DPS + Lingering Burn)
  - *Zealot Frenzy Aura* (+50% Shield Capacity + Allied Speed Aura)

### 🔬 Expanded Research Trees
- **UNSC Field Armory**:
  - *Cybernetic Overdrive* (+15% Vehicle Speed & Fire Rate)
  - *Titanium-A Nanite Plating* (+20% Vehicle/Air HP)
  - *Neural Link Targeters* (+25% Infantry Range, LOS, Accuracy)
- **Covenant Temple**:
  - *Plasma Supercharge Matrix* (+20% Plasma Damage)
  - *Harmonic Shield Amplifiers* (+30% Shields & 50% Faster Shield Recharge)
  - *Zealot Battle Frenzy* (+20% Infantry Move & Attack Speed)

### 🛡️ Covenant Brute Chieftain Kinetic Deflector & Vortex Buff
- **Kinetic Deflection Shield**:
  - The Chieftain deploys a persistent 360-degree kinetic deflector field upon researching *Vortex Deflector War Hammer* (`cov_bruteChief_upgrade1`).
  - Deflects incoming ballistic and small-arms fire away from the Chieftain while charging or executing melee slams.
- **Graviton Singularity Shockwave**:
  - Dramatically buffed physical launch and knockback forces on Chieftain area shockwaves, violently hurling enemy squads and light vehicles across the combat zone.

### ⚡ UNSC Wolverine Dual Light Railgun Conversion
- **Anti-Armor Auxiliary Light Railgun**:
  - Researching *Volley II & Anti-Armor Railgun* (`unsc_wolverine_upgrade3`) now dynamically replaces the Wolverine's auxiliary grenade mortar with a high-velocity light railgun turret.
  - Fires armor-piercing kinetic rounds with heavy bonus damage against ground armor and defensive turrets, transforming the Wolverine into a lethal anti-air and armor-shredding hybrid.

### 🧠 Skirmish AI Overhaul
- Dynamic counter-building and expansion logic.
- Systematic tech upgrade progression (including automated Wolverine railgun and Chieftain deflector upgrades).
- Integration of high-tier walkers, stealth operatives, and super-heavy units in AI strike forces.
- Optimized difficulty scaling across Easy, Normal, Hard, and Legendary.

---

## Installation & Usage

1. Copy the `AI Slop Mod` directory into your Halo Wars Definitive Edition `Mods` folder:
   `...\steamapps\common\HaloWarsDE\Mods\AI Slop Mod`
2. Enable **AI Slop Mod** using the Halo Wars Mod Manager (Haruspis) or activate mod directory loading.
3. Launch *Halo Wars: Definitive Edition* and enjoy custom skirmish or campaign games!

---

## Quality Assurance & Stability

All data files, XML architectures, and tactical scripts are verified against strict schema standards:
- 100% Valid XML and `.tactics` syntax.
- Zero ID or String collision.
- Clean cross-references across all objects, squads, techs, and string tables.

---

## Changelog

For a full historical record of changes, see [CHANGELOG.md](./CHANGELOG.md).
