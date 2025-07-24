# Procedural Side-Quests
This is a classification of procedural quests (also known as missions, tasks, contracts, assignments, or orders) in video game RPGs. The goal is to collect **setting-neutral** concepts that game designers can use when developing quests for open-world RPGs.
## Introduction
The quests are described with the intended goal in mind—what the player character (PC) needs to accomplish—rather than prescribing how the goal must be achieved. This gives the PC the flexibility to complete the quest in whatever way they choose. For example, if the quest giver needs an antidote, the PC is free to gather, buy, steal, rob, manufacture, or grow it as they see fit (subject to constraints and consequences).

The **characteristics** used to describe the quests are:
- **Main Goal**: When is the quest considered complete?
- **Main Solutions**: Typical methods for achieving the quest's goal.
- **Main Archetypes**/Target Group: Who would the questgiver typically entrust with the quest?
- **Main Gameloops**: Which core gameloops are typically involved in the quest?
- **Main Minigames**: Which minigames are typically included?
- **Quest Origin**: How does the PC learn about the quest? (e.g., commissioned by a *Questgiver* (e.g., military supervisor), *Hearsay* (listen in passing), *Marketplace* (seeing demand), finding Notes (e.*g*., treasure map), seeing special Event (e.*g*., seeing a meteor coming down), finding a *ruin* or *derelict* (e.*g*., finding a derelict vehicle), ...)
* **Procedural template**: What is the abstract description of the quest? (e.g., Escort quests follow the template "Transport X from A to B")

Variants of a quest can be generated using:
- **Constraints**: Minimum or maximum **time**, **quantity**, restricted areas, or other limits required to complete the quest.
- **Twists**: Unexpected changes or complications during the quest (e.g., the main goal becomes unreachable - such as the escort or quest giver dying). 
- **Consequences**: If the quest is discovered by a faction, the PC may face punishment (e.g., legal prosecution, exile, etc.).

```dataview
TABLE WITHOUT ID
    link(file.name, replace(file.name, "Quests", "")) AS Name,
    replace(join(goal), "Goal", "") AS "Main Goal",
    replace(join(solution), "Solution", "") AS "Main Solutions",
    replace(join(gameloop), "Loops", "") AS "Main Gameloop"
FROM #sidequest
SORT file.name ASC
```

## References
1. [https://evilrobotgames.com/adventure-quest-or-mission-vocabulary/](https://evilrobotgames.com/adventure-quest-or-mission-vocabulary/)

