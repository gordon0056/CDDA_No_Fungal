# No Fungal

[![Validate JSON](https://github.com/gordon0056/CDDA_No_Fungal/actions/workflows/validate-json.yml/badge.svg)](https://github.com/gordon0056/CDDA_No_Fungal/actions/workflows/validate-json.yml)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0--1.0-lightgrey.svg)](LICENSE)

**Version compatibility**: Tested and works with Cataclysm: Dark Days Ahead `0.I (stable)` and recent experimental builds.

## Description

This mod completely removes **fungal monsters** and **fungal-related overmap locations** from the game.

- Removes all fungal species (`mon_fungaloid`, `mon_spore`, etc.)
- Blacklists overmap specials such as fungal forests and towers
- Applies universal region override to prevent future fungal spawns

This is useful for players who want to disable the fungal infection mechanics and their biome entirely.

## Installation

1. Download the latest release from [Releases](https://github.com/gordon0056/CDDA_No_Fungal/releases).
2. Extract the `No_Fungal` folder into your `data/mods/` directory.
3. Enable `No Fungal` in the mod list when creating a new world.
4. **Note**: This mod must be enabled *before* world generation to be effective.

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| 1.1.0 | 2026-07-08 | Updated compatibility to 0.I, added CI validation |
| 1.0.0 | - | Initial release: removes fungal monsters and overmap locations |

## Troubleshooting

**Q: Can I still spawn fungal monsters via debug menu?**
A: Yes. This mod only removes natural spawns. Debug commands bypass the blacklist by design.

**Q: I enabled the mod but fungal locations still appear.**
A: This mod only affects new worlds. You must enable it *before* world generation.

## Author

Created by [Gordon0056](https://github.com/gordon0056) and the CDDA community.

## License

This work is in the public domain ([CC0 1.0](LICENSE)).
