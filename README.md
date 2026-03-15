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
- 1,500 personal prestige and 1,000 dynasty prestige
- All Setite rulers suffer -100 opinion towards the player

---

### 2. Pilgrimage to Enoch

A multi-stage event chain (4 events) representing a spiritual journey through the Underworld to the ghost-city of Enoch. Navigate the Shadowlands, survive the Tempest, resist spectral whispers, and reach the gates of Enoch for powerful rewards.

**Requirements:** Nagaraja follower of Talmahera, Nagaraja Legacy 3 perk, advanced necromancy, active coterie. Costs 300 gold with a 100-year cooldown.

**Rewards:**
- Pilgrim of Enoch trait (+3 Learning, +0.25 necromancy lifestyle XP, +10 dread baseline)
- Up to 3,000 learning XP depending on choices

---

### 3. Send Childe to Enoch

A character interaction that sends a dynasty member on a one-way pilgrimage to serve the clan from the Underworld.

**Requirements:** Nagaraja ruler with Talmahera faith and Nagaraja Legacy 3 perk. The childe must be an adult Nagaraja courtier of the same dynasty who is not the primary heir.

**Rewards:**
- "Dutiful Sire" modifier (+20 dynasty opinion, +1.0 monthly dynasty prestige multiplier for 25 years)
- 500 dynasty prestige

---

### 4. Convene a Silent Conclave

An event chain representing a secret gathering of Nagaraja elders to exchange knowledge and perform dark rituals, with potential masquerade risks.

**Requirements:** Nagaraja ruler with Nagaraja Legacy 2 perk. Costs 150 gold with a 20-year cooldown.

**Choices:**
- Focus the conclave on intrigue or necromancy
- Generous or token offering (with stress tradeoffs)
- 25% chance of masquerade exposure requiring gold or risk

**Modifiers:**
- Silent Conclave Insight: +2 Intrigue, -10 hostile scheme success chance (15 years)
- Silent Conclave Offering: +2 Learning, +0.15 necromancy lifestyle XP (15 years)

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
│   ├── decisions/                # 4 gameplay decisions
│   ├── modifiers/                # 9 character/event modifiers
│   ├── nicknames/                # Scourge of Sutekh nickname
│   ├── on_action/                # Flesh-Eater random event trigger
│   ├── scripted_character_templates/  # Itarajana Sorcerer template
│   └── traits/                   # Pilgrim of Enoch & Itarajana Sorcerer traits
├── events/                       # 13 events across all feature chains
├── localization/english/         # All English localization files
├── descriptor.mod
└── nagaraja_submod.mod
```

---

## Installation

Place the `nagaraja_submod` folder and its `.mod` file into your CK3 mod directory. Ensure the Princes of Darkness mod is installed and loaded before this submod.

## Compatibility

This submod uses unique event IDs (`podnagaraja.*`) and does not override any base PoD files, ensuring compatibility with other submods.
