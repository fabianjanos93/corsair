# Corsair Development Roadmap & TODOs

This document tracks upcoming design tasks, mechanical balances, lore expansions, and chapter overhauls across the *Corsair* rulebook and GM toolkit.

---

## 1. Class Gear Lore & Origins: MANTLEs
* **Concept:** **MANTLE** (*Modular Adaptive Neural Transmission Linked Equipment*) — the specialized, neural-interfaced tactical rigs worn by Corsair operatives across all classes.
* **Lore Deep-Dive Needed:**
  * **Origins & Creation:** How MANTLEs were originally conceived and engineered during the early expansion era. Who invented the initial neural transmission architecture (e.g., Precursor shard reverse-engineering, Flotilla military skunkworks, or pioneering neural cyberneticists during the Arrival)?
  * **Current State in 518 AA:** How MANTLE rigs are fabricated, standardized, customized, and maintained across the moons of the Sphere today.
  * **Class Integration:** Deepen how each class interfaces with their specialized MANTLE rig (e.g., Conduit capacitor plates, Pilot exodrone links, Weaver bio-filaments, etc.).
* **Target Files:**
  * [.agents/skills/corsair-class-design/SKILL.md](file:///c:/Users/csisz/IdeaProjects/corsair/.agents/skills/corsair-class-design/SKILL.md)
  * [.agents/skills/corsair-core-lore/SKILL.md](file:///c:/Users/csisz/IdeaProjects/corsair/.agents/skills/corsair-core-lore/SKILL.md)
  * [rulebook/classes/](file:///c:/Users/csisz/IdeaProjects/corsair/rulebook/classes/)

---

## 2. Feats / Traits System Rework: Removing Unlock Requirements [COMPLETED]
* **Summary:** Streamlined the Trait progression model. Removed all unlock requirements, challenge gates, and prerequisite trees. Traits are now categorized into operational areas and purchased directly with flat XP (costs 2–8 XP) during character creation or downtime training.
* **Character Creation XP Integration:** Replaced isolated "Skill Points" with flat Experience Points (6 XP baseline; +4 XP for Humans [10 total], +2 XP for Human-mixed races [8 total]). Starting XP can be spent freely on Skills (2 XP per level) or Traits.
* **Updated Files:**
  * [rulebook/character/Traits.md](file:///c:/Users/csisz/IdeaProjects/corsair/rulebook/character/Traits.md)
  * [rulebook/character/Creation.md](file:///c:/Users/csisz/IdeaProjects/corsair/rulebook/character/Creation.md)
  * [rulebook/character/Advancement.md](file:///c:/Users/csisz/IdeaProjects/corsair/rulebook/character/Advancement.md)
  * [rulebook/character/Player_Characters.md](file:///c:/Users/csisz/IdeaProjects/corsair/rulebook/character/Player_Characters.md)
  * [rulebook/character/Character_Sheet.html](file:///c:/Users/csisz/IdeaProjects/corsair/rulebook/character/Character_Sheet.html)

---

## 3. Conduit Class Balance: Amped Shot (Flame)
* **Problem:** In [Conduit.md](file:///c:/Users/csisz/IdeaProjects/corsair/rulebook/classes/Conduit.md#L91) and [Conduit_Sheet.html](file:///c:/Users/csisz/IdeaProjects/corsair/rulebook/classes/Conduit_Sheet.html), the **Flame** rider on `Amped Shot` currently grants a flat damage bonus per active Charge (`+1 Damage Bonus per active Charge`).
* **Fix Required:** Change the Flame branch to **boost the attack roll** itself (e.g., granting bonus dice, upgrades, or accuracy enhancements to the ranged attack test) rather than flat weapon damage, differentiating it from melee thermal backblast and preserving ranged damage curves.
* **Target Files:**
  * [rulebook/classes/Conduit.md](file:///c:/Users/csisz/IdeaProjects/corsair/rulebook/classes/Conduit.md#L91)
  * [rulebook/classes/Conduit_Sheet.html](file:///c:/Users/csisz/IdeaProjects/corsair/rulebook/classes/Conduit_Sheet.html)

---

## 4. GM Guide: Stealth & Infiltration
* **Concept:** Create a comprehensive Game Master reference chapter detailing stealth, security architecture, sensor networks, and infiltration missions.
* **Topics to Cover:**
  * **Sensor Suites & Detection:** Optical cameras, infrared heat sensors, acoustic sniffers, biometric scanners, and magnetic hull sensors.
  * **Fail-Forward & Turn Economy:** Expanding the *"Activating Actors"* principle when stealth tests fail, advancing security posture without grinding the infiltration to an immediate halt.
  * **Alert Tracks & Security Response:** Tiered alarm states (Unaware, Cautious, High Alert, Lockdown) and rapid response unit countdown tracks.
  * **Pacing Transitions:** Flowing smoothly between Place-to-Place scouting and Moment-to-Moment stealth breaches.
* **Target Files:**
  * `rulebook/gm/Stealth_and_Infiltration.md` *(New File)*
  * [rulebook/gm/Running_the_Game.md](file:///c:/Users/csisz/IdeaProjects/corsair/rulebook/gm/Running_the_Game.md)
