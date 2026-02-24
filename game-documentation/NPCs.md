---
title: NPCs
description: 
published: true
date: 2026-02-24T14:20:45.816Z
tags: 
editor: markdown
dateCreated: 2024-12-11T03:15:43.217Z
---

# NPCs

**NPCs (non-player characters)** in SCP Architect X serve many functions for your foundation.  
**NPCs are meant to be predictable and have limited random properties or decisions unless explicitly stated.**

---

## Current NPCs

This is a list of current NPCs within the game, their function, and cost to hire.

| **NPC Name** | **Function** | **Cost** |
|--------------|--------------|----------|
| Scientist | Performs tests using test subjects. | $1000+ |
| Security | Required for testing Euclid humanoid SCPs. | $1500+ |
| Test Subject | Required for tests to occur. Automatically hired when an old bed is placed. | Free |

---

## NPC Metrics

NPCs have 3 major metrics: **Bathroom, Hunger, & Energy.**

| **Metric** | **Description** |
|------------|----------------|
| Bathroom | Shows accessibility and use of toilets for NPCs. To increase this metric, place more toilets across your facility. |
| Hunger | Shows accessibility and use of cafeteria tables for NPCs. To increase this metric, place and link more cafeterias across your facility. |
| Energy | Shows the amount of rest and use of beds for NPCs. To increase this metric, ensure all staff and test subjects have a sufficient number of beds. |

You can view your overall NPC metrics by visiting the  
[Foundation Management](https://wikix.scparchitect.com/en/game-documentation/foundation-management) tab.

---

## NPC Prices

The cost of hiring Scientists and Security grows exponentially as you hire more.

1. The base cost for Scientists is **$1000**
2. The base cost for Security is **$1500**

---

### Pricing Formula

Where:

- `c` = base cost (1000 for Scientist, 1500 for Security)  
- `n` = number of NPCs of that type you already own  

This function raises 1.4 (the growth rate) to the power of `n`, multiplies it by `c`, and rounds to a whole number.

Think of `c` as the base cost, and `1.4^n` as the inflation multiplier that increases the price each time you hire another NPC.

---

### Total Cost of Buying n NPCs

This represents the geometric series sum of all purchases up to `n`.

---

# NPC Behavior

Outlined below is the static behavior of every NPC.

An NPC's lifecycle is a loop of actions and decisions it will make during its lifetime (from hiring to firing).
