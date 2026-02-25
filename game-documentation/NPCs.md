---
title: NPCs
description: 
published: true
date: 2026-02-25T05:30:55.109Z
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
| Test Subject | Required for tests to occur. Automatically hired when an D-Class Bed is placed. | Free |

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

`f(n)`

The static multipliers in `f(n)` are:
  1: 1,
	2: 5,
	3: 10,
	4: 15,
	5: 20,
	6: 25,
	7: 30,
	8: 35,
	9: 40,
	10: 50,
	11: 60,
	12: 80,
	13: 100,
	14: 150,
	15: 200,
	16: 400,
	17: 500,
	18: 600,
	19: 800,
	20: 1000,

 So at `17` NPCs a multiplier of `500` is applied to the NPC's based cost.
 For example, the `17th` scientist `($1000)` will cost `500 x 1000` = `$500,000`

---

### Total Cost of Buying n NPCs

This represents the geometric series sum of all purchases up to `n`.

---

# NPC Behavior

Outlined below is the static behavior of every NPC.

An NPC's lifecycle is a loop of actions and decisions it will make during its lifetime (from hiring to firing).
