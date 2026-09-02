# Changelog - AI Slop Mod

All notable changes to the **AI Slop Mod** for *Halo Wars: Definitive Edition* will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.1.0] - 2026-09-02

### Theme: Chieftain Kinetic Deflector & Wolverine Dual Railgun Conversion

This iteration brings explosive tactical weapon overhauls and leader combat enhancements to both UNSC and Covenant forces, dramatically increasing combat versatility against armor and small arms:

---

### Key Highlights & Additions

#### 1. Covenant: Brute Chieftain Kinetic Deflector & Shockwave Overhaul
- **Kinetic Deflector Shield** (`Deflect_01`):
  - Equipped the Brute Chieftain with a persistent 360-degree kinetic deflector field (`DeflectChanceMin/Max 0.65`, `DeflectDamageFactor 0.33`).
  - Deflects incoming ballistic and small-arms fire away from the Chieftain while charging or executing melee strikes.
  - Automatically unlocked upon researching **Vortex Deflector War Hammer** (`cov_bruteChief_upgrade1`).
- **Graviton Singularity Shockwave Buff**:
  - Significantly buffed physical launch and knockback forces on `AreaStunHammer` (launch angles increased to 15°–35°, impulse forces up to 600–900).
  - Ground units caught in the shockwave are thrown violently across the battlefield with true cinematic gravity impact.
  - Updated Chieftain upgrade strings (IDs `60150`, `60151`, `60154`, `60155`) with full lore and mechanical documentation.

#### 2. UNSC: Wolverine Dual Light Railgun Secondary Weapon Conversion
- **Anti-Armor Light Railgun** (`RailgunSecondary`):
  - Upgrading the Wolverine to **Volley II & Anti-Armor Railgun** (`unsc_wolverine_upgrade3`) now converts its auxiliary weapon mount from the standard anti-infantry grenade launcher into a hyper-velocity light railgun turret.
  - Fires armor-piercing kinetic projectiles (`fx_proj_lightRailgun_02` with `unsc_lightcannon_01` impacts) delivering 180 DPS at 60 max range.
  - Prioritizes enemy ground vehicles and fortified defensive turrets, transforming the Wolverine into a formidable dual-role anti-air and mobile armor-piercing vehicle.
  - Seamlessly reconfigures weapon action bindings in `unsc_veh_wolverine_01.tactics` and `techs.xml` upon research.
  - Documented in localized strings (IDs `60152`, `60153`).

#### 3. Skirmish AI Tech Priorities
- Added prioritized research rules in `data/aidata/techupgrades.ai` for UNSC Wolverine upgrades (`unsc_wolverine_upgrade1/2/3`) and Brute Chieftain upgrade paths, ensuring AI commanders aggressively field the new railgun and deflector tech.

---

## [1.0.0] - 2026-09-02

### Theme: Cybernetic Overcharge & Skirmish AI Overhaul

Welcome to the initial major release of **AI Slop Mod**! This update introduces brand new mechanized and infiltration unit squads, extensive tech tree expansions, an advanced skirmish AI combat overhaul, custom English string localization, and balanced combat mechanics for both the UNSC and Covenant factions.

---

### Key Highlights & Additions

#### 1. New UNSC Unit: Vanguard Heavy Mech (`unsc_inf_vanguardMech_01`)
- **Role**: Heavy Anti-Armor & Siege Walker.
- **Trained At**: UNSC Vehicle Depot (`unsc_bldg_vehicledepot_01`) [Position 8].
- **Combat Stats**: 4,500 Hitpoints, 1,500 Base Shieldpoints, 145 DPS, 60 LOS, Land Velocity 12.
- **Armament**: Twin High-Velocity Autocannons dealing medium explosive kinetic damage with bonus damage against heavy ground vehicles and fortifications.
- **Tactical Abilities**: Integrated Nanite Aegis shield generator, automated field repair capability for damaged allied mechanized units, capture point securing, and transport embarkation.
- **Upgrade Tree (Vehicle Depot - Pos 8)**:
  1. `Hydraulic Overdrive Servos`: +25% Movement Speed, +15% Hitpoints.
  2. `Depleted Uranium Autocannon`: +35% Autocannon DPS, heavy armor shredding.
  3. `Reactive Nanite Shield`: +50% Shield Capacity (+1,500 Shieldpoints), +20% Hitpoints.

#### 2. New Covenant Unit: Shadow Zealot Vanguard (`cov_inf_shadowZealot_01`)
- **Role**: Stealth Infiltration & Commander/Backline Assassin.
- **Trained At**: Covenant Hall (`cov_bldg_barracks_01`) [Position 8].
- **Squad Composition**: 2 Sangheili Shadow Zealots per squad.
- **Combat Stats**: 2,200 Hitpoints, 3,000 Shieldpoints, 170 DPS, 60 LOS, Land Velocity 16.
- **Armament**: Dual Superheated Energy Swords with rapid melee attack cycle.
- **Tactical Abilities**: Active optical camouflage cloak (`fx_cloakElite`), high mobility hit-and-run strikes, capture point securing, and Spirit transport garrisoning.
- **Upgrade Tree (Covenant Hall - Pos 8)**:
  1. `Adaptive Thermoptic Cloak`: +20% Movement Speed and continuous active camouflage.
  2. `Plasma-Infused Blades`: +40% Melee DPS with lingering thermal plasma burn.
  3. `Zealot Frenzy Aura`: +50% Shield Capacity and combat frenzy bonus to surrounding allied infantry.

#### 3. New Global Faction Research Techs
##### UNSC (Field Armory):
- **Cybernetic Overdrive** (`unsc_tech_cyberneticOverdrive`): +15% Speed and +15% Weapon Damage across all UNSC vehicles (Scorpion, Wolverine, Cobra) and Vanguard Mechs.
- **Titanium-A Nanite Plating** (`unsc_tech_titaniumPlating`): +20% Maximum Hitpoints across all UNSC vehicles, aircraft (Hornet, Vulture), and Vanguard Mechs.
- **Neural Link Targeters** (`unsc_tech_neuralInterface`): +25% Range/LOS and +15% Weapon Damage for Marines, ODSTs, and Spartans.

##### Covenant (Temple):
- **Plasma Supercharge Matrix** (`cov_tech_plasmaOvercharge`): +20% Plasma Weapon Damage for Ghosts, Wraiths, Banshees, and Grunts.
- **Harmonic Shield Amplifiers** (`cov_tech_harmonicShields`): +30% Shield Capacity for Elite Commandos and Shadow Zealots, +150% Shield Regeneration Rate, -50% Shield Recharge Delay for the faction.
- **Zealot Battle Frenzy** (`cov_tech_zealotFrenzy`): +20% Movement Velocity and +15% Damage across Grunts, Jackals, Hunters, and Shadow Zealots.

#### 4. Skirmish AI Overhaul
- **Dynamic Training Lists**: Integrated `unsc_inf_vanguardMech_01` and `cov_inf_shadowZealot_01` into AI strike groups and counter-attack waves.
- **Tech Upgrade Prioritization**: AI systematically researches new Vanguard Mech, Shadow Zealot, and global faction upgrades in `techupgrades.ai`.
- **Strategic Micro & Build Orders**: Overhauled building progression tables (`unscbuildlists.ai`, `covbuildlists.ai`) for faster expansions and defensive turret fortifications.
- **Balanced Difficulty Scaling**: Fine-tuned `aidifficultysettings.xml` for competitive pacing across Easy, Normal, Hard, and Legendary skirmish matches.

#### 5. Stringtable Localization & Lore
- Added localized English strings (`_locID` 60101 – 60142) in `stringtable-en.xml` for all new units, tactical roles, rollover descriptions, and tech tooltips.

---

### Files Modified & Created

```
AI Slop Mod/
├── data/
│   ├── aidata/
│   │   ├── covbuildlists.ai
│   │   ├── covtrainlists.ai
│   │   ├── techupgrades.ai
│   │   ├── unscbuildlists.ai
│   │   └── unsctrainlists.ai
│   ├── aidifficultysettings.xml
│   ├── objects.xml
│   ├── squads.xml
│   ├── stringtable-en.xml
│   ├── tactics/
│   │   ├── cov_inf_shadowZealot_01.tactics
│   │   └── unsc_inf_vanguardMech_01.tactics
│   └── techs.xml
├── CHANGELOG.md
└── README.md
```
