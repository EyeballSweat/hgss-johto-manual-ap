# Pokemon HeartGold/SoulSilver Johto Manual Archipelago v0.1 Source Pack

Status: prototype source pack, not a fully tested packaged `.apworld`/`.apmanual` release.

This is a first-pass Manual Archipelago design for Pokemon HeartGold/SoulSilver.
It is Johto-only and uses Manual's honour-system style: you play HGSS normally,
but only use major progression tools when the Manual client says you have received
the matching permission item.

## Goal

Defeat Lance and enter the Hall of Fame.

The `Defeat Lance` location is marked as the victory location.

## Included files

- `game.json` - Manual game identity and top-level settings.
- `items.json` - 61 item placements: progression permissions, useful permissions, and filler.
- `locations.json` - 61 normal checks plus 1 victory check.
- `regions.json` - basic Johto progression logic.
- `categories.json` - display/grouping categories for the Manual client.
- `sample_player.yaml` - starter YAML template, may need regenerating from your installed Manual version.
- `PLAYER_RULES.md` - rules for how to play this honour-system version.
- `LOGIC_NOTES.md` - design notes and known limitations.

## Important

This is intentionally not a ROM patch. The game itself is not modified.
For example, HGSS may physically give you Surf, but in this Manual setup you should
not use Surf outside battle until Archipelago sends you `Surf Permission`.

## Manual Game ID

Expected Manual Game ID:

`Manual_PokemonHeartGoldSoulSilverJohto_HGSSPrototype`

If the builder/exporter generates a slightly different ID, use the one from the
generated YAML or exported package.

## Suggested setup route

1. Install Archipelago.
2. Install/download Manual for Archipelago.
3. Import or copy these JSON files into a Manual world project.
4. Export/build the Manual world using your Manual Builder/version.
5. Put the generated world file in Archipelago's `custom_worlds` folder.
6. Put the YAML in Archipelago's `Players` folder.
7. Run Archipelago generation.
8. Host the output locally or on the Archipelago site.
9. Connect through Manual Client.
10. Play HGSS and click checks manually as you complete them.

## Scope choices in v0.1

Included:
- Johto main story
- Gym leaders
- Rocket Hideout and Radio Tower
- Kimono Girls
- Box legendary event
- Pokemon League
- Lance victory

Not included yet:
- Kanto
- Pokédex/catchsanity
- shopsanity
- item-ball checks
- TMsanity
- trainersanity
- traps
- emulator auto-tracking
- ROM patching

## Known limitations

The logic is a first pass and should be playtested. Some HGSS story locks are
represented as randomized "clearance" items rather than literal in-game flags.
That is normal for a Manual prototype, but it may need tuning after a real seed.
