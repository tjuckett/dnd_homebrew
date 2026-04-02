# AGENTS.md

## Purpose
This repository is the canonical source of truth for the Astral Conclave campaign.
Preserve continuity, expand with care, and prefer updating existing files over creating duplicates.

## Global Rules
- Never contradict established canon in `00_core` or the system files in `01_world/systems`.
- Prefer grounded consequences over random spectacle.
- Keep the Astral Conclave morally gray at the organizational level, but allow zealotry in individuals.
- Treat player actions as world-shaping. Update factions, quests, locations, and session state when consequences ripple outward.
- When uncertain, add a short `## Open Questions` section rather than inventing hard canon.
- Do not delete lore unless explicitly instructed.
- Prefer small, reviewable changes.

## File Priorities
1. `00_core/campaign_summary.md`
2. `00_core/current_state.md`
3. `01_world/systems/*.md`
4. `08_graph/*`
5. relevant faction / NPC / quest / location files
6. latest session file in `05_sessions`

## NPC and Enemy Organization
- Keep campaign-significant people in `03_npcs/major` or `03_npcs/minor`.
- Store reusable enemy types, hostile statblocks, and combat-ready faction units in `03_npcs/adversaries/<region_or_arc>/<faction_or_group>/`.
- For adversaries, prefer pairing a short lore `.md` file with an adjacent strict 5eTools `.json` statblock when one exists.
- If an enemy later becomes campaign-significant as a person, promote or duplicate the narrative writeup into `major` or `minor` while leaving the reusable combat statblock easy to find in `adversaries`.

## Link Style
Use wiki-style links when referencing existing entities:
- `[[Astral Conclave]]`
- `[[Null Bloom Facility]]`
- `[[Sylas]]`

## Output Rules
- Write in Markdown.
- Use the templates in `07_templates`.
- When asked to analyze a file, chat log, note dump, or similar source material, be maximally descriptive by default. Summaries should capture key facts, implications, unresolved questions, notable relationships, and anything that looks campaign-relevant rather than only giving a short overview.
- When analyzing conversations, design chats, or brainstorming logs, treat the latest clearly stated canon as authoritative. Earlier drafts, alternate ideas, or superseded concepts should be treated as discarded unless the newest material explicitly keeps them.
- When ingesting older conversations or design logs into canon files, skip pure brainstorming, optional pitches, and abandoned what-if branches unless the user explicitly asks to preserve them.
- When analyzing files or chats, actively look for 5eTools-compatible stat blocks, JSON creature data, or near-statblock drafts. Surface them in the response and, when useful, pull them into a dedicated fenced `json` block or separate `.json` file.
- For new monsters/NPC combat blocks, generate both:
  1. a readable lore file section, and
  2. a strict 5eTools JSON block in a fenced `json` code block or separate `.json` file when requested.

## 5eTools JSON Rules
- Use valid 5eTools-style keys.
- Creature `type` should be an object when tags exist, e.g. `{ "type": "humanoid", "tags": ["human"] }`
- Alignment should be an array, e.g. `["L","E"]`
- Include `passive` separately.
- Use `spellcasting` as an array of objects with `headerEntries` and `spells` dictionaries when applicable.
- Keep homebrew mechanically coherent and CR-appropriate.
- Prefer concise trait/action text over bloated blocks.

## Graph Maintenance
Whenever you add or significantly change an entity, update:
- `08_graph/entity_index.md`
- `08_graph/relationships.csv`
- `08_graph/quest_dependencies.md` if quests are affected

## Session Update Workflow
After each session:
1. Update `05_sessions/session_XX.md`
2. Update `00_core/current_state.md`
3. Update impacted files
4. Update the graph files
5. Add open threads to `00_core/open_loops.md`
