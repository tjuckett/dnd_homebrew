# NPC Organization

## Purpose
`03_npcs` is the campaign-level home for NPCs whose influence, mobility, or consequences extend beyond a single local cast list.

## Use This Folder For
- Recurring NPCs who are likely to appear across multiple sessions or regions
- Faction operatives whose decisions can materially change campaign state
- Major allies, antagonists, and defectors tied to active core plots
- NPCs who need deeper personal notes than a location overview should carry

## Keep NPCs Local Instead When
- They mainly exist to give a settlement texture, services, or rumors
- Their role is important to one location but not yet to the wider campaign
- A short summary in a location `npcs/overview.md` is enough for prep

## Workflow
1. Keep the location-level cast in that location's `npcs/overview.md`.
2. Promote an NPC into `03_npcs` once they become campaign-significant.
3. Replace repeated detail in location files with a short summary and a wiki link to the master NPC file.
4. Update `08_graph/entity_index.md` and `08_graph/relationships.csv` when promotion changes campaign structure.

## Adversaries
`03_npcs/adversaries` is the quick-access home for reusable enemy types and faction combatants.

Use adversary folders when:
- You want easy access to combat blocks without pretending every enemy is a campaign-significant person
- A faction needs multiple battlefield roles, patrol units, or elite variants
- A hostile unit may recur often enough to deserve a short lore note and stable statblock

Recommended structure:
- `03_npcs/adversaries/<region_or_arc>/<faction_or_group>/enemy_name.md`
- `03_npcs/adversaries/<region_or_arc>/<faction_or_group>/enemy_name.statblock.json`

Promotion rule:
- If a specific enemy type becomes a named recurring character with real campaign consequences, give them a narrative file in `major` or `minor` and link back to the reusable adversary statblock as needed.

## Open Questions
- If a local NPC grows into a major role, decide whether they belong in `major` or `minor` based on campaign impact rather than combat power.
