# Logic Notes - HGSS Johto Manual AP v0.1

## Counts

- Non-victory locations: 61
- Victory locations: 1
- Total item placements: 61

## Main progression chain

1. New Bark / Cherrygrove / Violet early game
2. Zephyr Badge opens Route 32 and Union Cave
3. Azalea and Slowpoke Well
4. Hive Badge + Cut Permission opens Ilex Forest and Goldenrod
5. Plain Badge + SquirtBottle opens Sudowoodo and Ecruteak
6. Fog Badge + Surf Permission opens Cianwood/Lake of Rage progression
7. Lake of Rage Clearance opens Rocket Hideout
8. Rocket Hideout Clearance opens Pryce
9. Glacier Badge starts Radio Tower logic
10. Rocket Uniform + Basement Key + Card Key progress through Radio Tower
11. Radio Tower Clearance + RageCandyBar Clearance + Strength Permission opens Ice Path/Blackthorn
12. Rising Badge + Whirlpool Permission opens Dragons Den
13. Dragons Den Clearance + Waterfall Permission + Kimono/Legendary/Elite Four clearances opens Victory Road and the League

## Deliberate simplifications

- E4 members are all in the Pokemon League region and are not individually gated.
- Kanto is excluded.
- The box legendary is represented by `Legendary Clearance`, not by species/version.
- The Master Ball itself is a location check, not a randomized progression item.
- Some story events are represented as AP items because this is not a ROM patch.

## Likely future improvements

- Split Olivine and Cianwood logic more accurately.
- Add version-specific Ho-Oh/Lugia wording.
- Add optional Kanto expansion.
- Add catchsanity/fishsanity categories.
- Add item-ball checks if the scope needs to become larger.
- Replace some clearance items with Manual `events.json` if you want tighter story sequencing.
