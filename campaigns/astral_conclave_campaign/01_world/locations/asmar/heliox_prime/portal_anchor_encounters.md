# Central Spire Portal-Anchor Encounters

All monster mechanics are bundled in [Heliox Portal Encounter Stat Blocks](../../../../06_assets/gameplay/heliox_portal_encounter_statblocks.md), with a single 5eTools import file containing every required creature.

## Core Structure
- The portal has `3` anchor systems:
  - West Anchor,
  - East Anchor,
  - Upper Anchor.
- Each system can be disabled from either of two locations:
  - its physical anchor on Level `2`,
  - or its control station on Level `3`.
- This creates `6` possible interaction locations.
- Disabling a physical anchor and its own matching control station still counts as disabling only one anchor system.
- The party must take two different anchor systems offline.
- Once two systems are offline:
  - the `Null-Key Shroud` loses quorum,
  - the real portal accepts an Aetherbind wrist-device connection,
  - and one character can spend an uninterrupted round closing it.

## Six Interaction Locations At A Glance

| System | Physical location | Control location | Main pressure | Relative risk |
|---|---|---|---|---|
| West | Level 2 west floor anchor | Level 3 west station | Controlled civilian screen | High moral risk |
| East | Level 2 east floor anchor | Level 3 east station | Heavy machinery and reinforcements | High combat risk |
| Upper | Suspended above Level 2 | Level 3 north station | Vertical exposure and portal pull | High environmental risk |

## Difference Between The Two Methods
### Control-Station Disable
- Quieter and safer for creatures in transit.
- Requires access to the station followed by an orderly standby command.
- Usually takes two actions:
  1. authenticate or bypass the station,
  2. place its anchor into standby.
- The phase key automatically passes authentication.
- Without it, use a DC `17` Arcana, Investigation, or Tinker's Tools check.
- A failed check triggers the station's local defense but does not permanently lock the party out.
- A station-disabled anchor can be reactivated by a Conclave technician unless the party:
  - remains to defend the console,
  - physically jams it,
  - removes its control crystal,
  - or destroys the linked station after the safe shutdown completes.

### Physical-Anchor Disable
- Louder, faster, and permanent.
- The anchor can be destroyed through damage or sabotaged at close range.
- Suggested shared statistics:
  - AC `18`,
  - `60` hit points,
  - damage threshold `10`,
  - resistance to nonmagical bludgeoning, piercing, and slashing damage,
  - immunity to poison and psychic damage.
- Instead of dealing damage, a character adjacent to an anchor can accumulate `2` sabotage successes using DC `17` Arcana or Tinker's Tools checks.
- A failed sabotage check releases an anchor-specific hazard.
- A destroyed anchor cannot be restored during the encounter.
- Destruction makes the final wrist-device closure more violent, but it still works.

## Presenting The Six Choices
- The Continuity Audit Chamber should display three paired systems rather than six unrelated targets.
- Suggested interface:

```text
WEST SYSTEM
  PHYSICAL ANCHOR: LEVEL 2
  CONTROL STATION: LEVEL 3

EAST SYSTEM
  PHYSICAL ANCHOR: LEVEL 2
  CONTROL STATION: LEVEL 3

UPPER SYSTEM
  PHYSICAL ANCHOR: LEVEL 2/3 SUSPENSION
  CONTROL STATION: LEVEL 3

PORTAL SECURITY QUORUM: 2 OF 3 REQUIRED
WRIST CLOSURE: DENIED WHILE QUORUM HOLDS
```

- When a player selects a system, the display highlights both ways to disable it.
- If they select a station and its matching physical anchor, display:
  - `WARNING: BOTH TARGETS GOVERN THE SAME ANCHOR SYSTEM.`
- This prevents the players from spending time disabling two locations that only count as one objective.

## Conclave-Wide Contingencies
### 1. Redundancy Transfer
- When the first anchor system goes offline, the remaining two flare with visible violet energy.
- The portal remains open and the Shroud remains active.
- Effects:
  - the Conclave immediately knows which system was lost,
  - all remaining anchor hazards deal one additional damage die,
  - and technicians abandon nonessential duties to reinforce likely second targets.

### 2. Adaptive Lockdown
- The first disabled system triggers segmented shutters between Levels `2`, `3`, and `4`.
- The Conclave does not seal every route at once; it seals the most direct path from the first target to a different anchor system.
- The party can:
  - force the shutter,
  - use the service lift,
  - cross through the portal gallery,
  - or exploit a Sovereign-access route.
- This makes the second objective tactically different without forcing a specific path.

### 3. Station Reactivation Teams
- A station placed into standby is a soft disable.
- One [[Astral Conclave Field Technician]] and controlled assistants attempt to reach it.
- A technician adjacent to the station can restore it with two actions.
- Removing the control crystal or succeeding on an additional DC `17` tool check makes the station irrecoverable for the encounter.
- This forces the party to decide whether to defend a captured station, sabotage it permanently, or race the restoration clock.

### 4. Controlled Civilian Repair Orders
- The Conclave can command civilians to shield, cool, or reconnect damaged anchor machinery.
- Citizens do not need technical expertise; the network feeds them simple movements.
- Treat them as a moral obstruction rather than effective engineers:
  - they grant half cover to an anchor,
  - impose disadvantage on reckless ranged attacks,
  - or remove one sabotage success if left uninterrupted for a round.
- The Local Directive Projector ends this contingency by latching its Emergency Dormancy Protocol; affected citizens release the machinery and shut down in place.

### 5. Last-Lock Capacitor
- The Conclave keeps one emergency capacitor beside the Upper Control Station.
- It cannot replace a disabled anchor or keep the portal stable.
- When the second anchor system goes offline, it keeps the `Null-Key Shroud` alive until the end of the next round.
- The party sees:
  - `ANCHOR QUORUM LOST.`
  - `LAST-LOCK DISCHARGE ACTIVE.`
  - `WRIST CLOSURE AVAILABLE IN 1 ROUND.`
- The capacitor can be destroyed early:
  - AC `17`,
  - `25` hit points,
  - immunity to poison and psychic damage.
- This contingency gives the Conclave one final reaction without invalidating the two-anchor objective.

### 6. Closure Interruption
- Once wrist closure begins, every Conclave defender understands that it is the final point of failure.
- They focus on:
  - breaking the user's wrist-device connection,
  - moving the user out of range,
  - forcing the user through the portal,
  - reactivating a soft-disabled station,
  - or destroying the Local Directive Projector before it can latch the dormancy command onto newly arriving civilians.
- The closing character must remain conscious, within portal-control range, and able to use the wrist device until the start of their next turn.

### 7. Scuttle Surge
- A Conclave handler can use a reaction when a physical anchor is destroyed.
- The destroyed anchor dumps its remaining charge into the portal chamber.
- Creatures within `20 feet` make a DC `16` Dexterity saving throw:
  - failure: `4d8` lightning damage and pushed `10 feet`,
  - success: half damage and no push.
- Controlled citizens caught by the Local Directive Projector automatically release the overloading anchor and shut down in place.

### 8. Accelerated Intake
- After the first anchor system goes offline, the Conclave increases the portal intake rate.
- Advance the civilian casualty or transfer clock by one additional step if the party spends an entire round without progressing toward a second system.
- This discourages resting after the first objective without requiring arbitrary reinforcements.

## Mobile Conclave Response Pool
- Do not populate all six locations with full encounters simultaneously.
- Only the two locations selected by the party should receive complete combat rosters.
- Defenders assigned to unused nodes remain busy protecting their own systems and do not all converge into one impossible battle.
- The mobile response consists of the second-target pursuit package defined below.
- Veyr-Kas can appear by projection without adding another creature to initiative.
- Defeated enemies are not replaced unless the portal explicitly brings reinforcements from its destination.

## Encounter Balance
### Party Assumption
- Built for `5` characters at level `10`.
- Still appropriate for level `11` using the scaling package below.
- Uses the 2014 encounter thresholds as a rough reference:

| Party | Medium | Hard | Deadly |
|---|---:|---:|---:|
| Five level-10 characters | `6,000 XP` | `9,500 XP` | `14,000 XP` |
| Five level-11 characters | `8,000 XP` | `12,000 XP` | `18,000 XP` |

- Adjusted XP is only an estimate. Forced movement, portal hazards, civilian protection, station objectives, and inability to rest make these encounters harder than their monster totals indicate.

### Design Target
- Each location is intentionally overloaded while its controlled Heliox defenders remain active.
- Full-roster adjusted XP ranges from `14,000-20,000`, deadly for a level-10 party and potentially deadly for level `11`.
- This is not permission to run every defender as a normal stand-up fight. The apparent imbalance is the clue: deploying the Local Directive Projector removes the unwilling Heliox from combat.
- After the dormancy directive takes hold, only loyal Conclave personnel remain active. Their adjusted XP ranges from approximately `5,400-9,600`, leaving a medium encounter, or a hard encounter at the Upper Control Station.
- The second chosen location adds the pursuit package, but its Heliox Sever-Axe is also susceptible to the projector and shuts down when the dormancy pulse reaches it.
- Remaining resources, loyal spellcasters, overcharged hazards, and closure pressure make the two-location sequence life-threatening without requiring the party to kill controlled Heliox citizens.
- The encounters are not intended to be followed by a third full node battle.
- Once two different anchor systems are offline, shift immediately into the Last-Lock and wrist-closure finale.
- A short rest between objectives is technically possible, but it advances the intake clock to completion and allows the Conclave to evacuate most remaining personnel and captives.
- In normal play, the party should have time for potions, healing spells, and a few quick actions, but not a short rest.

### Second-Target Pursuit Package
- After the first anchor system goes offline, add these creatures to whichever second location the party chooses:
  - `1` [[Heliox Sever-Axe]] (CR `4`).
- Narrative role:
  - the Sever-Axe hunts intruders, blocks access, and keeps the party from immediately reaching the second objective.
- These creatures arrive from Level `4`, the service lift, or the nearest sealed route.
- They should be visible approaching or shown on the audit display so the escalation feels earned.

### Level-11 Adjustment
- If the party is level `11`, add `1` [[Astral Conclave Veil Escort]] (CR `2`) to the second-target pursuit package.
- If the level-11 party is already injured or low on spells, omit this additional escort.
- If the level-10 party is highly optimized or still near full resources, add the Veil Escort as well.
- If the level-10 party reaches the second location badly depleted, run the base roster without the Sever-Axe.

### Controlled Heliox Combat Constructs
- Heliox constructs in these encounters are victims of the same control network as the populace.
- The Local Directive Projector carries a locked emergency-dormancy directive; the party cannot replace it with an attack or sabotage order.
- When the stationary field activates, each network-controlled Heliox construct and citizen within `60 feet` immediately releases all grapples and restraints, ends concentration, and shuts down in place.
- An affected creature becomes incapacitated, has speed `0`, and is removed from initiative.
- The emergency directive latches for `10 minutes`, so moving an inert creature beyond the field does not restore the fivefold command.
- Affected Heliox do not attack the Conclave, damage anchors, operate stations, move, communicate, provide intentional cover, or help the party.
- Their inert bodies can still provide ordinary physical cover or obstruct a narrow route. Moving one requires the normal effort appropriate to its size and weight.
- Astral Conclave humanoids are unaffected unless they carry compatible control hardware.
- The loyal Conclave casters know what the projector does. They prioritize counterspelling attempts to protect it, forcing its carrier away from deployment points, and damaging it before the field opens.

### Running The Deliberate Overload
- Before initiative, distinguish the unwilling Heliox from the loyal defenders on the map or audit display. The players should understand which enemies the projector can remove.
- Let the full roster demonstrate its danger for at most one round if the party delays deployment; do not focus every attack on a single character before they can act.
- Controlled Heliox prioritize grapples, blocking, and forced movement over killing blows. Loyal Conclave casters provide the lethal pressure.
- Once the field opens, immediately remove affected Heliox from the combat tracker. Leave their tokens in place as inert terrain.
- If the party refuses to use the projector, run the full deadly roster honestly, but clearly preserve routes for retreat, later deployment, or surrender through the portal.

### Concrete Encounter Rosters

| Location | Full defenders before override | Full adjusted XP | Loyal defenders after Heliox shut down | Post-override adjusted XP |
|---|---|---:|---|---:|
| West Physical Anchor | Security Construct, Forge-Hammer, Runebinder, Veil Escort, Null Cantor, Relay Handler | `15,300` | Veil Escort, Null Cantor, Relay Handler | `5,900` |
| East Physical Anchor | Engine Overseer, Security Construct, Crystal Technician, `2` Field Technicians, Rift Magister | `15,000` | `2` Field Technicians, Rift Magister | `5,400` |
| Upper Physical Anchor | Harpoon Gunner, Runebinder, `2` Veil Escorts, Relay Handler, Null Cantor | `14,000` | `2` Veil Escorts, Relay Handler, Null Cantor | `7,400` |
| West Control Station | Runebinder, Security Construct, Forge-Hammer, Relay Handler, Null Cantor, Veil Escort | `15,300` | Relay Handler, Null Cantor, Veil Escort | `5,900` |
| East Control Station | Arm Operator, Security Construct, Harpoon Gunner, Relay Handler, Rift Magister, Veil Escort | `16,300` | Relay Handler, Rift Magister, Veil Escort | `6,900` |
| Upper Control Station | Dual-Forge Brute, Runebinder, Forge-Hammer, Relay Handler, Null Cantor, Rift Magister | `20,000` | Relay Handler, Null Cantor, Rift Magister | `9,600` |

- Do not add the second-target pursuit package to the first encounter.
- Do not add unrelated crowd monsters to the XP budget. Use controlled civilians as objectives and hazards.
- If the party divides into two groups simultaneously, see the split-party adjustment below instead of using both full rosters unchanged.

## Encounter 1: West Physical Anchor
### Identity
- Moral-pressure encounter.
- The west anchor is partially enclosed by the controlled citizen intake lane.
- The Conclave deliberately routes civilians between the party and the machinery.

### Terrain
- Anchor sits on a raised `3-foot` plinth.
- Controlled citizens occupy two adjacent crowd zones.
- Narrow maintenance trench behind the anchor provides access for sabotage.
- Portal pulses push loose objects toward the threshold.

### Suggested Defenders
- `1` [[Heliox Security Construct]] (CR `5`).
- `1` [[Heliox Forge-Hammer]] (CR `4`).
- `1` [[Heliox Runebinder]] (CR `5`).
- `1` [[Astral Conclave Veil Escort]] (CR `2`).
- `1` [[Astral Conclave Null Cantor]] (CR `5`).
- `1` [[Astral Conclave Relay Handler]] (CR `3`).
- Controlled citizens remain crowd hazards rather than individual monsters.
- If this is the second objective, add the pursuit package.

### Monster Tactics
- The Security Construct holds the maintenance-trench entrance and uses Shield Bash to push characters back into the crowd.
- The Forge-Hammer grapples anyone attempting sabotage and pins them beside the pulsing anchor.
- The Runebinder uses Web or Rune Snare to keep characters in the repulsion-pulse area and saves Counterspell for attempts to bypass the anchor defenses.
- The Veil Escort stays behind the civilian line, uses Veil Screen to obscure the anchor, and targets the Local Directive Projector when possible.
- The Null Cantor opens with Slow and uses Signal Fracture against the projector carrier and anyone moving toward the maintenance trench.
- The Relay Handler snares characters outside the projector's intended deployment point.
- When the field opens, all three Heliox constructs release any held creatures and shut down in place; the Cantor, Handler, and Escort remain.

### Anchor Hazard: Repulsion Pulse
- At initiative count `20`, the west anchor emits a force pulse.
- Creatures within `20 feet` make a DC `16` Strength saving throw or are pushed `10 feet`.
- After the first anchor system goes offline, the push increases to `15 feet` and can knock creatures prone.

### Conclave Contingency
- **Citizens As Armor:** Controlled citizens are commanded to physically cover access panels.
- The party must move, restrain, or locally override them before sabotage can begin safely.
- Attacking through them risks civilian casualties.

### Best Solutions
- Use the Local Directive Projector to shut down the controlled defenders; move an inert body only if it blocks the maintenance trench.
- Have a strong character move the Security Construct while a technician sabotages the anchor.
- Use forced movement or terrain control to clear the maintenance trench nonlethally.

### Reward
- Disabling this anchor opens the west equipment-bypass lane as a route toward the Upper Anchor or Level `3` stair.

## Encounter 2: East Physical Anchor
### Identity
- Heavy combat and machinery encounter.
- The east anchor sits beside the Conclave equipment-bypass route and repair stockpiles.

### Terrain
- Suspended cargo rails cross above the anchor.
- Charged component crates provide cover but explode if heavily damaged.
- Magnetic repair arms can grab creatures or anchor components.
- The service lift is nearby, allowing reinforcements from Level `4`.

### Suggested Defenders
- `1` [[Heliox Engine Overseer]] (CR `6`).
- `1` [[Heliox Security Construct]] (CR `5`).
- `1` [[Heliox Crystal Technician]] (CR `3`).
- `2` [[Astral Conclave Field Technician]]s (CR `1` each).
- `1` [[Astral Conclave Rift Magister]] (CR `6`).
- If this is the second objective, add the pursuit package.

### Monster Tactics
- The Engine Overseer remains beside the anchor, gains temporary hit points from its linked console, and uses Emergency Repairs after the anchor takes meaningful damage.
- The Security Construct holds the equipment-lane chokepoint and pushes characters away from the anchor's access panels.
- The Crystal Technician uses Crystal Scatter to slow anyone approaching through the equipment lane.
- Field Technicians remain in cover, repairing the anchor or removing sabotage progress instead of maximizing damage.
- If threatened, one Field Technician uses a purge crystal on the destination logs while the other continues repairs.
- The controlled Heliox constructs can be overridden; the organic Field Technicians cannot.
- The Rift Magister uses Gravitic Fold and Vector Step to keep the projector carrier away from a clear deployment point.
- Once the field opens, the Overseer, Security Construct, and Crystal Technician shut down where they stand. The Magister and Field Technicians continue defending and repairing the anchor.

### Anchor Hazard: Magnetic Draw
- At initiative count `20`, creatures wearing metal armor or carrying large metal weapons within `25 feet` make a DC `16` Strength saving throw.
- On a failure, they are pulled `10 feet` toward the anchor or knocked prone against nearby machinery.

### Conclave Contingency
- **Rapid Repair:** A Field Technician adjacent to the anchor can restore `15` hit points or remove one sabotage success as an action.
- Destroying the repair crane or separating technicians from the anchor ends this contingency.

### Best Solutions
- Drop cargo to block the service-lift reinforcement path.
- Turn the magnetic arms against the Mauler.
- Split between controlling technicians and damaging the anchor.

### Reward
- Captured repair tools grant advantage on one later physical-anchor sabotage check.

## Encounter 3: Upper Physical Anchor
### Identity
- Vertical movement and falling-hazard encounter.
- The anchor hangs above the portal threshold from three articulated support arms connected to Level `3`.

### Terrain
- Two narrow maintenance catwalks approach it from the gallery.
- The Level `2` floor is `25 feet` below the catwalks.
- The active portal pulls loose objects and falling creatures toward its threshold.
- Support chains and conduits provide climbable routes.

### Suggested Defenders
- `1` [[Heliox Harpoon Gunner]] (CR `5`).
- `1` [[Heliox Runebinder]] (CR `5`).
- `2` [[Astral Conclave Veil Escort]]s (CR `2` each).
- `1` [[Astral Conclave Relay Handler]] (CR `3`).
- `1` [[Astral Conclave Null Cantor]] (CR `5`).
- If this is the second objective, add the pursuit package at the nearest gallery entrance.

### Monster Tactics
- The Harpoon Gunner stays braced near the north suspension point and uses Hookshot to pull characters off safe catwalk positions.
- The Runebinder uses Web across one catwalk and Counterspell against flight or teleportation that would trivialize the approach.
- One Veil Escort screens the Gunner while the other crosses between catwalks to threaten climbers.
- The Relay Handler uses Signal Snare on grouped characters, ideally immediately before a portal-draw pulse.
- The Null Cantor uses Slow on climbers and Counterspell against flight, teleportation, or magical protection placed around the projector.
- When the field opens, the Harpoon Gunner and Runebinder shut down on the catwalks; the loyal Escorts, Handler, and Cantor remain.
- The enemies retreat toward the Upper Control Station if the physical anchor becomes irrecoverable.

### Anchor Hazard: Portal Draw
- At initiative count `20`, exposed creatures on the catwalks make a DC `16` Strength or Dexterity saving throw.
- On a failure, they slide `10 feet` toward the portal-facing edge.
- A creature already at the edge falls unless secured.

### Conclave Contingency
- **Deadfall Release:** When the anchor falls below half hit points, the handler can release one support arm.
- The anchor swings across a catwalk:
  - DC `16` Dexterity save,
  - `3d10` bludgeoning damage on failure,
  - and possible fall.
- If all support arms are cut without controlling the descent, the anchor crashes into the portal floor and advances the civilian casualty clock.

### Best Solutions
- Reach it by climbing rather than using both defended catwalks.
- Secure the anchor with ropes or magic before destroying supports.
- Capture the suspension controls and lower it away from the crowd.

### Reward
- Controlled lowering creates heavy cover on Level `2` and blocks one citizen intake lane without harming civilians.

## Encounter 4: West Control Station
### Identity
- Stealth, console access, and narrow-balcony defense.
- This is the least heavily staffed station but the easiest one for the Conclave to isolate with shutters.

### Terrain
- Station occupies a small west gallery overlooking the portal chamber.
- Two security shutters can trap intruders at the console.
- A narrow maintenance ledge connects toward the destination-log room.
- The open portal floor lies below the railing.

### Suggested Defenders
- `1` [[Heliox Runebinder]] (CR `5`).
- `1` [[Heliox Security Construct]] (CR `5`).
- `1` [[Heliox Forge-Hammer]] (CR `4`).
- `1` [[Astral Conclave Relay Handler]] (CR `3`).
- `1` [[Astral Conclave Null Cantor]] (CR `5`).
- `1` [[Astral Conclave Veil Escort]] (CR `2`).
- If this is the second objective, add the pursuit package outside the isolation shutters.

### Monster Tactics
- The Runebinder opens with Web or Rune Snare to keep characters away from the console.
- It saves Counterspell for magic that would bypass the station or remove a major restraint.
- The Security Construct holds the shutter entrance and uses Intercept against anyone trying to pass toward the station.
- The Forge-Hammer guards the console and uses Anvil Lock on the first character who reaches it.
- The Relay Handler stays within relay range for Redirect Pulse and uses Signal Snare if the party groups inside the shutters.
- The Null Cantor remains behind the shutters, using Slow and Counterspell to delay deployment of the projector.
- The Veil Escort protects the Cantor and uses Veil Screen to hide the console.
- If the station is placed into standby, the Relay Handler prioritizes reactivation over dealing damage.
- When the projector field opens, the Runebinder, Security Construct, and Forge-Hammer shut down in place. The loyal Conclave trio continues the defense.

### Station Hazard: Countercommand Arc
- A failed access check triggers a DC `16` Intelligence saving throw.
- On a failure, the user loses reactions until the start of their next turn and involuntarily steps `5 feet` away from the console.
- Constructs hear the command as their own internal voice.

### Conclave Contingency
- **Isolation Shutters:** The station seals after the standby command begins.
- This protects the operator from outside attackers but may separate them from the party.
- The shutters open when the sequence completes or can be forced with DC `18` Athletics.

### Best Solutions
- Enter stealthily and disable the local alarm before touching the console.
- Let one character operate while another prevents the handler from restoring access.
- Remove the station's control crystal before leaving.

### Reward
- Destination logs reveal whether citizens are arriving alive at the portal's far side.

## Encounter 5: East Control Station
### Identity
- Reinforcement and identity-spoofing encounter.
- Located beside the service lift and portal-handler workspace.

### Terrain
- Wide enough for a small skirmish but crossed by lift tracks and cable channels.
- Service-lift doors can open behind the party.
- Console has clear sight to the Local Directive Projector deployment area below.
- A maintenance crane can move equipment between Levels `3` and `2`.

### Suggested Defenders
- `1` [[Heliox Arm Operator]] (CR `4`).
- `1` [[Heliox Security Construct]] (CR `5`).
- `1` [[Heliox Harpoon Gunner]] (CR `5`).
- `1` [[Astral Conclave Relay Handler]] (CR `3`).
- `1` [[Astral Conclave Rift Magister]] (CR `6`).
- `1` [[Astral Conclave Veil Escort]] (CR `2`).
- If this is the second objective, the pursuit package arrives through the lift.

### Monster Tactics
- The Security Construct blocks the console approach and punishes attempts to move past it.
- The Arm Operator uses Clamp and Toss to throw characters away from the console or over the gallery rail.
- The Harpoon Gunner fires from beside the lift and pulls characters back across the gallery after they pass the Security Construct.
- The Relay Handler uses Signal Snare near the lift doors and attempts to lock the projector's emitter vanes before deployment.
- The Rift Magister uses Gravitic Fold to pull the projector carrier toward the lift tracks and uses Banishment only if an ally can seize the dropped device.
- The Veil Escort screens the Magister and projector-targeting defenders.
- If the projector field reaches the gallery, all three Heliox defenders release any held creatures and shut down; the Handler, Magister, and Escort remain.
- Once the station enters standby, surviving defenders attempt to hold the party until lift reinforcements arrive.

### Station Hazard: Sanctuary Lockout
- The east station can broadcast a false maintenance interlock to the projector.
- Once per encounter, the handler forces the projector carrier to make a DC `16` Intelligence saving throw when attempting deployment.
- On a failure, the emitter vanes remain locked until the carrier or an adjacent character uses an action to clear the interlock with a DC `16` Arcana or Tinker's Tools check.

### Conclave Contingency
- **Lift Reinforcement:** When combat begins, the lift displays an incoming car arriving in `2` rounds.
- The party can:
  - jam the doors,
  - redirect the car,
  - drop it to Level `1`,
  - or prepare for the mobile response team.

### Best Solutions
- Disable or exploit the lift before beginning the station sequence.
- Take the Relay Handler alive to obtain the phase key.
- Use the crane to carry a character or the projector between floors.

### Reward
- The phase key bypasses authentication at any other control station and disables identifier spoofing.

## Encounter 6: Upper Control Station
### Identity
- Highest-security station and best location for the final confrontation.
- It controls the suspended anchor and sits nearest the `Null-Key Shroud` and Last-Lock Capacitor.

### Terrain
- North gallery directly above the portal arch.
- Two narrow approaches from east and west.
- Upper-anchor access bridge crosses open space.
- Shroud console and capacitor provide hard cover.
- Portal energy creates intermittent low gravity.

### Suggested Defenders
- `1` [[Heliox Dual-Forge Brute]] (CR `6`).
- `1` [[Heliox Runebinder]] (CR `5`).
- `1` [[Heliox Forge-Hammer]] (CR `4`).
- `1` [[Astral Conclave Relay Handler]] (CR `3`).
- `1` [[Astral Conclave Null Cantor]] (CR `5`).
- `1` [[Astral Conclave Rift Magister]] (CR `6`).
- Veyr-Kas may appear by projection and issue commands but does not add another combatant.
- If this is the second objective, add the pursuit package from the east or west approach.
- Use controlled citizens below as encounter pressure rather than adding more creatures here.

### Monster Tactics
- The Dual-Forge Brute controls the center approach and uses Thermal Clash when at least two characters reach the station or capacitor.
- The Runebinder stays near the Shroud, uses Web or Ice Storm to split the two approaches, and saves Counterspell for attempts to disable the capacitor instantly.
- The Forge-Hammer holds the capacitor side of the gallery and grapples anyone attempting to reach it.
- The Relay Handler operates the station, activates Last-Lock, and only attacks when no console action is urgent.
- The Null Cantor suppresses the party's magic and saves Counterspell for effects protecting or transporting the projector.
- The Rift Magister uses forced movement to prevent the party from deploying the projector near all three Heliox defenders at once.
- When the second anchor system goes offline, every defender focuses on preventing wrist closure rather than fighting to the death.
- When the projector field opens, all three Heliox defenders shut down in place. The Handler and both loyal casters form the final defense and flee through the portal only if Last-Lock fails.

### Station Hazard: Authority Reversal
- The first character who accesses the station without a phase key must make a DC `17` Charisma saving throw.
- On a failure, the station marks them as an unauthorized asset:
  - Conclave creatures have advantage on their next attack against that character,
  - and the projector treats their square as an unsafe deployment point until the mark is purged, preventing the field from being opened within `10 feet` of them.

### Conclave Contingency
- **Last-Lock Defense:** If this is the second disabled system, the capacitor activates immediately.
- The handler uses the extra round to:
  - attack the wrist-device user,
  - reactivate a soft-disabled station,
  - or jump through the portal with the destination logs.
- Destroying the capacitor removes that final round of protection.

### Best Solutions
- Approach from both sides of the gallery.
- Steal the phase key before touching the console.
- Separate the technician from the capacitor.
- Drop onto the station from the upper-anchor maintenance structure.

### Reward
- Capturing this location provides:
  - the cleanest portal destination data,
  - control of the Last-Lock Capacitor,
  - and the strongest evidence that the Conclave designed the Null-Key Shroud specifically against the party.

## Recommended Encounter Flow
### If The Party Stays Together
1. Let them choose one of the six locations from the audit display.
2. Present the first objective as deliberately overwhelming until the projector shuts down its controlled Heliox defenders.
3. Trigger redundancy transfer and adaptive lockdown.
4. Show reinforcements moving toward the most obvious second target.
5. Let the party change plans based on that information.
6. Run the second objective with the pursuit package and loyal spellcasters pressuring projector deployment.
7. Trigger the Last-Lock Capacitor.
8. Begin the one-round wrist-device closure finale.

### If The Party Splits
- Each group targets a different anchor system.
- Alternate between groups at the same initiative count.
- Do not run two full encounter rosters against split groups.
- At each chosen location:
  - keep the highest-CR monster,
  - keep one support creature,
  - remove all other base monsters.
- Do not deploy the pursuit package unless one group finishes early and reinforcements can logically reach the other.
- When either group causes an alarm, the other location receives warning but not immediate reinforcements.
- Both groups can time their disabling actions so the Shroud drops at a chosen moment.
- The group nearest the portal begins wrist closure while the other prevents station reactivation.

### If They Target A Station And Matching Anchor
- Warn them through the audit display that both locations control the same system.
- If they proceed anyway:
  - disabling the station lowers the matching physical anchor's defenses,
  - the anchor loses its damage threshold and resistances,
  - but taking both out still counts as only one disabled system.
- This keeps the choice useful without letting it satisfy both required objectives.

## Recommended Two-Target Combinations
- **Safest for civilians:** West Station plus East Station.
- **Fastest physical route:** West Anchor plus East Anchor.
- **Most cinematic:** Upper Anchor plus East Station.
- **Best stealth route:** West Station plus Upper Station.
- **Best use of mobility:** Upper Anchor plus West Station.
- **Most dangerous:** East Anchor plus Upper Station, because it combines the Mauler fight with the best-defended console.

## Open Questions
- Which defenders survived earlier encounters and should be removed from the response pool?
- Is Veyr-Kas physically present or only directing the defense remotely?
- How many citizens are already inside the Level `2` chamber when the first anchor goes offline?
- Can the construct PC use Sovereign authority to bypass one station check automatically?
- Does the party know the difference between a soft station disable and permanent anchor destruction before committing?
