---
name: corsair-equipment-design
description: >-
  Design guidelines, mathematical invariants, naming conventions, load tiering, and upgrade economics for designing or overhauling Equipment (Melee, Firearms, Armor, Gear) in Corsair.
---

# Corsair Equipment Design System

This skill documents the design principles, mathematical rules, naming conventions, and economic frameworks for authoring and balancing equipment in Corsair. Use this skill whenever designing or revising items in **Melee**, **Firearms**, **Armor**, and **Gear**.

---

## 1. Mathematical Invariants: Zero-Division Rule

* **No Division Formulas:** Never use mathematical division (e.g., `STR/2`, `STR/3`, or `(Agility / 3) + 1`).
* **Flat Integer Scaling:** All weapon bonuses, armor protections, and stat requirements must use flat integer additions (`+1`, `+2`, `+3`, etc.) or direct attribute references (e.g., *"equal to the lower attribute of the test"*).
* **Threshold Requirements:** Physical scaling should use minimum attribute thresholds (e.g., **Min STR 4**) with clear binary handling rules for Melee weapons and Shields (e.g., 1H melee weapons require two hands if below Min STR; 2H melee weapons cannot be wielded; shields require Min STR). Firearms do not use Strength thresholds, relying instead on 1H vs. 2H handling, Rate of Fire (RoF), and Range Band Accuracy. Armor does not use Strength thresholds, relying instead on Load encumbrance, tactical properties, and **Cumbersome (X)** Agility Downgrades.

---

## 2. Naming Conventions: D&D-Style Functional Archetypes

* **Clear Archetypes Over Model Numbers:** Primary equipment tables must use recognizable, functional archetype names (e.g., *Combat Knife, Boarding Axe, Shotgun, Assault Rifle, Heavy Armor, Riot Shield*) rather than cluttered in-universe make/model strings (*"KSK Sharkfin"*, *"VWS Scrapper"*).
* **Separation of Lore and Mechanics:** In-universe manufacturer lore (Panthera Arms, Vandal's Workshop, Caldera Foundry, Ker'Satz Korp, Chidori-Qwei) belongs in introductory text or flavor descriptions, keeping catalog tables clean and easy to scan during play.

---

## 3. Load Tiering & Weight Class Guidelines

* **Structured Load Progression:** Organize equipment across flexible Load tiers (e.g., `Load 1/2`, `1`, `2`, `3`, `4+`) to reflect increasing bulk, power, and character investment.
* **Symmetry Across Types:** Within each load tier of a weapon category, provide balanced options across different damage types, delivery methods, or tactical roles.
* **Proportional Scaling:** Higher Load should correlate with greater flat damage bonuses, protection values, or tactical utility. Armor scales with `Protection = Load + 1` across standard baselines, with heavier suits taking on properties.

---

## 4. Escalating Upgrade Kit Economics (+1 Equivalent)

Mastercrafted equipment upgrades represent high-end precision aerospace machining and custom armorer tuning.

* **Hard Cap:** A single piece of equipment can benefit from a maximum of **3 Upgrade Kits** (restricted to a maximum of **2 Upgrade Kits** for one-handed weapons).
* **Tiered Escalating Pricing:**
  * **Weapons (Melee & Firearms):**
    * **1st Upgrade:** `10,000 Credits`
    * **2nd Upgrade:** `25,000 Credits`
    * **3rd Upgrade:** `50,000 Credits`
  * **Armor (Premium Mil-Spec Customization):**
    * **1st Upgrade:** `50,000 Credits`
    * **2nd Upgrade:** `100,000 Credits`
    * **3rd Upgrade:** `180,000 Credits`
* **Permanent Choice Per Kit Applied:**
  * **Weapons:** Choose **Weight Reduction** (-1 Load, min 1/2) or **Performance Enhancement** (+1 Flat Damage Bonus).
  * **Armor:** Choose **Reinforced Plating** (+1 Protection), **Lightweight Composites** (-1 Load, min 1), or **Specialized Modification** (install Hardened, Blast-Dampened, Tactical Harness (1), or Muffled; cannot duplicate existing properties).

---

## 5. Rulebook Architecture & Document Hierarchy

* **`Equipment.md` as High-Level Hub:** Define universal concepts (e.g., Load capacity calculation `12 + (Strength × 2)`, general categories) in [Equipment.md](file:///c:/Users/csisz/IdeaProjects/corsair/rulebook/equipment/Equipment.md) and use direct markdown links to dedicated sub-chapter files.
* **Dedicated Sub-Chapter Files:** Detail specific mechanics, tables, and narrative examples in dedicated files:
  * [Melee.md](file:///c:/Users/csisz/IdeaProjects/corsair/rulebook/equipment/Melee.md)
  * [Firearms.md](file:///c:/Users/csisz/IdeaProjects/corsair/rulebook/equipment/Firearms.md)
  * [Armor.md](file:///c:/Users/csisz/IdeaProjects/corsair/rulebook/equipment/Armor.md)
  * [Gear.md](file:///c:/Users/csisz/IdeaProjects/corsair/rulebook/equipment/Gear.md)
* **Accompanying Printable Handouts:** Every major equipment category should maintain an A4 print-ready HTML reference sheet generated via the [`corsair-printable-sheets`](file:///c:/Users/csisz/IdeaProjects/corsair/.agents/skills/corsair-printable-sheets/SKILL.md) skill.
