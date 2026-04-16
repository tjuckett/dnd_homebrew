# 5eTools NPC Statblock Workflow

When asked to generate a combat-ready NPC or monster:

1. Write or update the lore Markdown file first if the creature is campaign-relevant.
2. Then produce strict 5eTools-compatible JSON.
3. Match the schema and field style already used in `Chaos Inc Homebrew.json`.

## Baseline Template
```json
{
  "name": "Example Name",
  "source": "ChaosIncHomebrew",
  "page": 0,
  "size": ["M"],
  "type": {
    "type": "humanoid",
    "tags": ["human"]
  },
  "alignment": ["L", "N"],
  "ac": [
    {
      "ac": 16,
      "from": ["breastplate"]
    }
  ],
  "hp": {
    "average": 85,
    "formula": "10d8 + 40"
  },
  "speed": {
    "walk": 30
  },
  "str": 12,
  "dex": 16,
  "con": 18,
  "int": 14,
  "wis": 13,
  "cha": 15,
  "save": {
    "dex": "+6",
    "con": "+7"
  },
  "skill": {
    "perception": "+4",
    "stealth": "+6"
  },
  "senses": [
    "darkvision 60 ft."
  ],
  "passive": 14,
  "languages": [
    "Common"
  ],
  "resist": [
    "necrotic"
  ],
  "conditionImmune": [
    "charmed"
  ],
  "cr": "7",
  "pb": "+3",
  "trait": [
    {
      "name": "Example Trait",
      "entries": [
        "Trait text."
      ]
    }
  ],
  "action": [
    {
      "name": "Multiattack",
      "entries": [
        "The creature makes two attacks."
      ]
    },
    {
      "name": "Example Weapon",
      "entries": [
        "{@atk mw} {@hit 6} to hit, reach 5 ft., one target. {@h}8 ({@damage 1d8 + 4}) slashing damage."
      ]
    }
  ],
  "bonus": [
    {
      "name": "Example Bonus Action",
      "entries": [
        "Bonus action text."
      ]
    }
  ],
  "reaction": [
    {
      "name": "Example Reaction",
      "entries": [
        "Reaction text."
      ]
    }
  ]
}
```

## Common Optional Sections
- `immune`
- `resist`
- `vulnerable`
- `conditionImmune`
- `spellcasting`
- `bonus`
- `reaction`
- `legendary`
- `legendaryActions`
- `traitTags`
- `actionTags`
- `senseTags`
- `languageTags`
- `miscTags`
- `damageTags`
- `conditionInflict`
- `legendaryGroup`
- `fluff`

Only include optional fields when they add value or are already being maintained for that statblock.

## Field Conventions
- Always use `source: "ChaosIncHomebrew"`.
- Prefer `ac` as an array of objects with `ac` and `from` instead of a bare number, because that is the dominant pattern in `Chaos Inc Homebrew.json`.
- Use `type` as a string only for very simple cases; prefer the object form when tags matter.
- Use uppercase size letters such as `["M"]`, `["L"]`, or `["G"]`.
- Keep `cr` as a string.
- Include `pb` when you are explicitly tuning by proficiency bonus or following the newer constructs/vehicle entries in the compendium.
- `passive` should usually reflect Perception.
- Skill keys should use 5eTools-style names such as `sleightOfHand`, not human-readable labels.

## Entry Formatting
- Keep rules text inside `entries` arrays.
- Use 5eTools inline tags in action text whenever possible:
  - `{@atk mw}`, `{@atk rw}`, `{@atk ms}`, `{@atk rs}`
  - `{@hit 7}`
  - `{@h}`
  - `{@damage 2d6 + 4}`
  - `{@dc 15}`
  - `{@condition prone}`
  - `{@spell counterspell}`
- Use plain `DC 15` only if you are matching an existing local file that already does so.
- Weapon and spell actions should be written in a way that can render cleanly in 5eTools without extra prose around them.

## Spellcasting Pattern
Use a `spellcasting` array when needed:

```json
"spellcasting": [
  {
    "name": "Spellcasting",
    "headerEntries": [
      "The creature is a 9th-level spellcaster. Its spellcasting ability is Intelligence (spell save {@dc 15}, {@hit 7} to hit with spell attacks). It has the following wizard spells prepared:"
    ],
    "spells": {
      "0": {
        "spells": [
          "{@spell fire bolt}",
          "{@spell mage hand}"
        ]
      },
      "1": {
        "slots": 4,
        "spells": [
          "{@spell mage armor}",
          "{@spell shield}"
        ]
      }
    },
    "ability": "int",
    "type": "spellcasting"
  }
]
```

## Legendary Actions Pattern
If the creature has legendary actions:

```json
"legendary": [
  {
    "name": "Attack",
    "entries": [
      "The creature makes one weapon attack."
    ]
  }
],
"legendaryActions": 3
```

## Quality Checklist
- JSON must be valid.
- The numbers should be internally consistent with CR and proficiency bonus.
- Attack bonuses, save DCs, and skill bonuses should match the listed stats unless there is a clear feature-based reason otherwise.
- Do not mix lore summary prose into the statblock JSON.
- Keep names, damage types, and keywords capitalized the way 5eTools expects.
- If you add nonstandard mechanics, make them readable in one pass at the table.
- Prefer clean, reusable statblocks over over-scripted encounter text.

## Practical Notes From Existing Files
- Older files may still reflect earlier source naming, but new and updated statblocks should use `ChaosIncHomebrew`.
- Some older files omit `pb`, `traitTags`, and other metadata; that is acceptable for lightweight NPCs.
- Some older files also use simpler `ac: [17]` formatting. That works, but the richer object form is the better default for new work.
- Vehicles, fortresses, and boss monsters may need subsystem traits, lair/legendary support, and more custom text than a standard humanoid NPC.
