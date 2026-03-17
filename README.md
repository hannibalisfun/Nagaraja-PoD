# Nagaraja: Sentinels of the Eastern Hand

**Version:** 1.0.0
**Supported Version:** 1.18.*
**Dependency:** Princes of Darkness (PoD)

A gameplay expansion submod for the Princes of Darkness mod that adds six major features exclusive to Nagaraja vampire characters, emphasizing their unique identity as flesh-eating necromancers and guardians of the Eastern Hand.

---

## Features

### 1. Purge the Serpent from India

A major objective decision allowing Nagaraja rulers to claim dominance over the Indian subcontinent by eliminating all Setite and Daitya rivals from India and Tibet.

**Requirements:** Independent Nagaraja ruler with 1,500+ prestige, 15+ counties, and capital in India or Tibet.

**Rewards:**
- "Scourge of Sutekh" nickname and modifier (+3 Martial, +10 hostile scheme duration, -10 murder scheme duration, +15 same faith opinion)
- 1,500 personal prestige and 1,000 renown
- All Setite rulers suffer -100 opinion towards the player

---

### 2. Pilgrimage to Enoch (Journey)

A POD Journey representing a once-in-a-lifetime spiritual pilgrimage through the Underworld to the ghost-city of Enoch. The journey features a planning phase (~2 years) followed by a travel phase where 4-5 encounters are randomly selected from a pool of 8 modular events, culminating in a fixed finale at the Gates of Enoch.

**Requirements:** Nagaraja follower of Talmahera, Nagaraja Legacy 3 perk, advanced necromancy. Costs 300 gold. Can only be undertaken once per character.

**Journey Structure:**
- **Planning Phase:** ~2 years of preparation
- **Travel Phase:** 4-5 randomly selected pool events spaced over ~1-2.5 years, followed by the Gates of Enoch finale

**Pool Events (8 total, 4-5 selected per journey):**
- **Entering the Shadowlands** — Open your senses to the dead (Learning check) for the Attuned to the Dead modifier
- **The Tempest** — Brave a spectral storm through prowess, necromancy, or patience
- **Whispers of the Drowned** — Command lost wraiths (Intrigue check), ignore them, or devour their ectoplasm
- **The False Necropolis** — Investigate a trap (Learning check), avoid it, or destroy it with advanced necromancy. Blocked if warned by the Wraith Market
- **A Spectral Anomaly** — Push through (Prowess check), go around, or study it (Learning check)
- **The Wraith Market** — Trade gold for intelligence and a warning, devour a wraith for prowess and dread, or pass through
- **Echoes of the Silk Road** — Search ghostly ruins (Learning check), speak with inhabitants (Diplomacy check), or record your findings
- **A Fellow Traveler** — Share intelligence freely (with a 15% spy follow-up risk), trade cautiously (Intrigue check), decline, or share supplies

**Final Event — Gates of Enoch:**
- Pay respects to the Del'Roh (Pilgrim of Enoch trait + 200 prestige + 200 renown)
- Study the libraries of Brujah (3,000 learning XP + 100 prestige)
- Remain and serve in Enoch (Pilgrim of Enoch trait + 500 renown + torpor)

---

### 3. Send Childe to Enoch

A character interaction that sends a dynasty member on a one-way pilgrimage to serve the clan from the Underworld.

**Requirements:** Nagaraja ruler with Talmahera faith and Nagaraja Legacy 3 perk. The childe must be an adult Nagaraja courtier of the same dynasty who is not the primary heir.

**Rewards:**
- "Dutiful Sire" modifier (+20 dynasty opinion, +1.0 monthly renown multiplier for 25 years)
- 500 renown

---

### 4. Convene a Silent Conclave

An event chain representing a secret gathering of Nagaraja elders to exchange knowledge and perform dark rituals, with potential masquerade risks.

**Requirements:** Nagaraja ruler with Nagaraja Legacy 2 perk. Costs 150 gold with a 20-year cooldown.

**Choices:**
- Focus the conclave on intrigue or necromancy
- Generous or token offering (with stress tradeoffs)
- 25% chance of masquerade exposure requiring gold or risk

**Modifiers:**
- Silent Conclave Insight: +2 Intrigue, -10% hostile scheme success chance (15 years)
- Silent Conclave Offering: +2 Learning, +15% necromancy lifestyle XP (15 years)

---

### 5. The Flesh-Eater's Risk

A recurring random event representing the dangerous feeding drive unique to Nagaraja, providing stress relief but with masquerade exposure risks.

**Trigger:** 10% chance every 45-150 days for Nagaraja characters (3-year cooldown per trigger).

**Feeding Options:**
- **Feed Carefully:** Low risk, -20 stress, +2 intrigue for 2 years
- **Feed Recklessly:** -40 stress, +2 prowess and +5 dread for 2 years, but 40% masquerade risk
- **Feed on Ghoul:** Safe but costs ghoul opinion
- **Endure Hunger:** +30 stress, 10% learning lifestyle XP for 2 years

If evidence is discovered, handle it by destroying it (30 gold), ignoring it (masquerade exposure), or framing someone else (intrigue check).

---

### 6. Recruit Itarajana Sorcerer

A decision-triggered event chain to recruit a ghoul practitioner of Itarajana (Hindu blood sorcery tradition) as a courtier.

**Requirements:** Nagaraja ruler with Talmahera faith, Nagaraja Legacy 1 perk, Learning 12+, capital in India/Tibet/Middle East/Central Asia. Maximum 3 sorcerers at court. Costs 75 gold with a 10-year cooldown.

**Sorcerer Details:**
- Generated with randomized age, culture, gender, and attributes
- Itarajana Sorcerer trait (+4 Learning, +2 Intrigue, +0.25 necromancy lifestyle XP)
- Follow-up event 2-5 years later offering research encouragement or knowledge exploitation

---

## File Structure

```
nagaraja_submod/
├── common/
│   ├── character_interactions/   # Send Childe interaction
│   ├── culture/innovations/      # Journey jank innovations (icon/illustration)
│   ├── decisions/                # 4 gameplay decisions
│   ├── modifiers/                # 19 character/event modifiers
│   ├── nicknames/                # Scourge of Sutekh nickname
│   ├── on_action/                # Flesh-Eater random event trigger
│   ├── scripted_character_templates/  # Itarajana Sorcerer template
│   ├── scripted_guis/            # Journey SGUIs (requirements, on_end, travel_phase)
│   └── traits/                   # Pilgrim of Enoch & Itarajana Sorcerer traits
├── events/                       # 21 events across all feature chains
├── localization/english/         # All English localization files
├── descriptor.mod
└── nagaraja_submod.mod
```

---

## Installation

Place the `nagaraja_submod` folder and its `.mod` file into your CK3 mod directory. Ensure the Princes of Darkness mod is installed and loaded before this submod.

## Compatibility

This submod uses unique event IDs (`podnagaraja.*`) and does not override any base PoD files, ensuring compatibility with other submods.
