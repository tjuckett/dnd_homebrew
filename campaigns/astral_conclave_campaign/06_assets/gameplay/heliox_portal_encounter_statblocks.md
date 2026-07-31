# Heliox Portal Encounter Stat Blocks

## 5eTools Import
- Table-facing roster sheet: [Heliox Portal Encounter Cheat Sheet](heliox_portal_encounter_cheat_sheet.md)
- Combined bestiary: [Heliox Portal Encounter Bestiary](heliox_portal_encounter_bestiary.json)
- Contains all `14` creature stat blocks required by the six anchor encounters and reinforcement packages.
- Source tag: `ChaosIncHomebrew`.

## Quick Reference

| Creature | CR | AC | HP | Primary function |
|---|---:|---:|---:|---|
| [[Astral Conclave Field Technician]] | `1` | `13` | `27` | Repairs, purge crystals, and station recovery |
| [[Astral Conclave Veil Escort]] | `2` | `15` | `44` | Mobile skirmisher, obscuring screen, handler protection |
| [[Astral Conclave Relay Handler]] | `3` | `14` | `52` | Restraint, command static, station operation |
| [[Heliox Crystal Technician]] | `3` | `15` | `68` | Slowing cone and volatile death burst |
| [[Astral Conclave Null Cantor]] | `5` | `15` | `82` | Countermagic, slowing effects, and concentration disruption |
| [[Astral Conclave Rift Magister]] | `6` | `16` | `104` | Planar magic, forced movement, and loyal defender repositioning |
| [[Heliox Forge-Hammer]] | `4` | `16` | `76` | Grapple and restrain characters at objectives |
| [[Heliox Sever-Axe]] | `4` | `17` | `85` | Second-target pursuit and aggressive pressure |
| [[Heliox Arm Operator]] | `4` | `17` | `95` | Pushes and throws characters away from consoles |
| [[Heliox Harpoon Gunner]] | `5` | `16` | `110` | Ranged damage and forced movement on catwalks |
| [[Heliox Runebinder]] | `5` | `16` | `99` | Spell control, restraint, and counterspell |
| [[Heliox Security Construct]] | `5` | `19` | `126` | Chokepoint defense and shield-based forced movement |
| [[Heliox Dual-Forge Brute]] | `6` | `16` | `114` | Heavy area damage and central approach denial |
| [[Heliox Engine Overseer]] | `6` | `18` | `135` | Anchor repairs, temporary hit points, and shock pulse |

## Source JSON Files
### Astral Conclave
- [Field Technician](../../03_npcs/adversaries/asmar/astral_conclave/astral_conclave_field_technician.statblock.json)
- [Relay Handler](../../03_npcs/adversaries/asmar/astral_conclave/astral_conclave_relay_handler.statblock.json)
- [Veil Escort](../../03_npcs/adversaries/asmar/astral_conclave/astral_conclave_veil_escort.statblock.json)
- [Null Cantor](../../03_npcs/adversaries/asmar/astral_conclave/astral_conclave_null_cantor.statblock.json)
- [Rift Magister](../../03_npcs/adversaries/asmar/astral_conclave/astral_conclave_rift_magister.statblock.json)

### Controlled Heliox Constructs
- [Arm Operator](../../03_npcs/adversaries/asmar/heliox_prime/heliox_arm_operator.statblock.json)
- [Crystal Technician](../../03_npcs/adversaries/asmar/heliox_prime/heliox_crystal_technician.statblock.json)
- [Dual-Forge Brute](../../03_npcs/adversaries/asmar/heliox_prime/heliox_dual_forge_brute.statblock.json)
- [Engine Overseer](../../03_npcs/adversaries/asmar/heliox_prime/heliox_engine_overseer.statblock.json)
- [Forge-Hammer](../../03_npcs/adversaries/asmar/heliox_prime/heliox_forge_hammer.statblock.json)
- [Harpoon Gunner](../../03_npcs/adversaries/asmar/heliox_prime/heliox_harpoon_gunner.statblock.json)
- [Runebinder](../../03_npcs/adversaries/asmar/heliox_prime/heliox_runebinder.statblock.json)
- [Security Construct](../../03_npcs/adversaries/asmar/heliox_prime/heliox_security_construct.statblock.json)
- [Sever-Axe](../../03_npcs/adversaries/asmar/heliox_prime/heliox_sever_axe.statblock.json)

## Encounter Rosters
### West Physical Anchor
- `1` Heliox Security Construct
- `1` Heliox Forge-Hammer
- `1` Heliox Runebinder
- `1` Astral Conclave Veil Escort
- `1` Astral Conclave Null Cantor
- `1` Astral Conclave Relay Handler

### East Physical Anchor
- `1` Heliox Engine Overseer
- `1` Heliox Security Construct
- `1` Heliox Crystal Technician
- `2` Astral Conclave Field Technicians
- `1` Astral Conclave Rift Magister

### Upper Physical Anchor
- `1` Heliox Harpoon Gunner
- `1` Heliox Runebinder
- `2` Astral Conclave Veil Escorts
- `1` Astral Conclave Relay Handler
- `1` Astral Conclave Null Cantor

### West Control Station
- `1` Heliox Runebinder
- `1` Heliox Security Construct
- `1` Heliox Forge-Hammer
- `1` Astral Conclave Relay Handler
- `1` Astral Conclave Null Cantor
- `1` Astral Conclave Veil Escort

### East Control Station
- `1` Heliox Arm Operator
- `1` Heliox Security Construct
- `1` Heliox Harpoon Gunner
- `1` Astral Conclave Relay Handler
- `1` Astral Conclave Rift Magister
- `1` Astral Conclave Veil Escort

### Upper Control Station
- `1` Heliox Dual-Forge Brute
- `1` Heliox Runebinder
- `1` Heliox Forge-Hammer
- `1` Astral Conclave Relay Handler
- `1` Astral Conclave Null Cantor
- `1` Astral Conclave Rift Magister

### Second-Target Pursuit Package
- Level `10` party:
  - `1` Heliox Sever-Axe
- Level `11` party:
  - add `1` Astral Conclave Veil Escort unless the party is already badly depleted.

## Control-Override Reminder
- Heliox constructs are controlled victims, not willing Conclave troops.
- A network-controlled Heliox construct caught within the deployed Local Directive Projector's `60-foot` field immediately loses its reaction and ceases hostile action.
- It immediately releases grapples and restraints, ends concentration, becomes incapacitated with speed `0`, and is removed from initiative.
- The shutdown remains latched for `10 minutes`, even if the inert creature is moved beyond the field.
- The command is factory-locked: affected Heliox cannot attack defenders, damage anchors, operate stations, move, communicate, or otherwise fight for the party.
- Leave its token in place; the inert body may provide physical cover or obstruct a narrow path.
- Astral Conclave creatures are unaffected unless they carry compatible control hardware.
