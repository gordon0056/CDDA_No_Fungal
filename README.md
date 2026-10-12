# No Fungal

[![Validate JSON](https://github.com/gordon0056/CDDA_No_Fungal/actions/workflows/validate-json.yml/badge.svg)](https://github.com/gordon0056/CDDA_No_Fungal/actions/workflows/validate-json.yml)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0--1.0-lightgrey.svg)](LICENSE)

**Version compatibility**:

| CDDA version | Mod folder | Notes |
|--------------|------------|-------|
| `0.H` / `0.I` (stable) | repo root (`modinfo.json` id `no_fungal`) | uses legacy `region_overlay` format |
| `0.J` (experimental) and newer | `No_Fungal_0J/` (id `no_fungal_0J`) | uses new `region_settings` format |

> The two formats are mutually incompatible: the legacy `region_overlay` type is an
> unrecognized object on 0.J+ (the game fails to load), and the new `region_settings`
> override requires `default_oter` on 0.H/0.I (the game fails to load there too).
> Pick exactly one folder matching your game version.

## Description

This mod completely removes **fungal monsters** and **fungal-related overmap locations** from the game.

- Removes all fungal species (`mon_fungaloid`, `mon_spore`, etc.)
- Blacklists overmap specials such as fungal forests and towers
- Applies universal region override to prevent future fungal spawns

This is useful for players who want to disable the fungal infection mechanics and their biome entirely.

## Installation

1. Download the latest release from [Releases](https://github.com/gordon0056/CDDA_No_Fungal/releases).
2. Pick the folder matching your game version (see compatibility table above):
   - **0.H / 0.I stable** → copy the repo-root files (`modinfo.json`, `monster_blacklist.json`, `region_settings.json`) into `data/mods/No_Fungal/`.
   - **0.J experimental and newer** → copy the `No_Fungal_0J/` folder contents into `data/mods/No_Fungal_0J/` (enable `No Fungal (0.J+)` in the mod list).
3. Enable the mod in the mod list when creating a new world.
4. **Note**: This mod must be enabled *before* world generation to be effective.

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| 2.0.0 | 2026-10-12 | Split into two variants: root stays on legacy `region_overlay` for 0.H/0.I, new `No_Fungal_0J/` folder with `region_settings` for 0.J+; added `version` fields; CI now validates nested JSON |
| 1.1.0 | 2026-07-08 | Updated compatibility to 0.I, added CI validation |
| 1.0.0 | - | Initial release: removes fungal monsters and overmap locations |

## FAQ

**Q: Does this mod affect existing worlds?**
A: No. This mod only affects world generation. Enable it before creating a new world.

**Q: Are fungal items and recipes also removed?**
A: No. This mod only removes monsters and overmap locations. Fungal gear and recipes remain in the game.

**Q: Can fungal enemies still appear through other means?**
A: Natural spawns and fungal biomes are fully blocked. Debug spawn commands will still work.

## Author

Created by [Gordon0056](https://github.com/gordon0056) and the CDDA community.

## License

This work is in the public domain ([CC0 1.0](LICENSE)).
