# 5eTools NPC Statblock Workflow

When asked to generate a combat-ready NPC or monster:

1. Write or update the lore Markdown file first.
2. Then produce strict 5eTools JSON.

## Required Output Shape
```json
{
  "name": "Example Name",
  "source": "Homebrew",
  "page": 0,
  "size": ["M"],
  "type": {
    "type": "humanoid",
    "tags": ["human"]
  },
  "alignment": ["L","E"],
  "ac": [16],
  "hp": {"average": 85, "formula": "10d8 + 40"},
  "speed": {"walk": 30},
  "str": 12,
  "dex": 16,
  "con": 18,
  "int": 14,
  "wis": 13,
  "cha": 15,
  "save": {"dex": "+6", "con": "+7"},
  "skill": {"arcana": "+5", "perception": "+4"},
  "passive": 14,
  "resist": ["necrotic"],
  "senses": ["darkvision 60 ft."],
  "languages": ["Common"],
  "cr": "7",
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
    }
  ]
}
```

## Additional Rules
- Keep JSON valid.
- Make CR believable.
- If spellcasting is needed, use a `spellcasting` array.
- Do not mix lore prose into JSON.
