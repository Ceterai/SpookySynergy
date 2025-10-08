# Changelog

All notable changes to this project will be documented in this file.

The format is loosely based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.1] - Haunted Bag Enhancement

### Added

- **Halloween mask patches**: Updates for rarity and pricing:
  - Patched 5 new Halloween mask variants (`hallowmask1-5`)
  - Patched 5 new Phobe mask variants (`phobemask1-5`)
  - Patched 3 new pumpkin head variants (`halhumanoidpump`, `halhylotlpump`, `halpumpkinhead`)

### Changed

- **Halloween Reward Treasure Pools**: Rebalanced item drop weights and fixed item parameters syntax:
  - Adjusted pool round probabilities: changed from [0.5, 0]/[0.5, 1] to [0.4, 0]/[0.6, 1]
  - Reduced Phobe mask weights from 0.2 to 0.15 each for better balance
  - Reduced pumpkin head weights from 0.1 to 0.08 each
  - Fixed item syntax for colored items: converted from `"parameters"` format to array format `[item, count, parameters]`
    - Fixed wizard hat color variants
    - Fixed monster head color variants (eye, mushroom, creeper, yeti, eyeball, lagoon, slime heads)
    - Fixed pirate head color variant

### Technical Additions

- **Metadata**: New meta files for Steam Workshop integration:
  - Added Steam Workshop description file (`.meta/description-steam.bbcode`)
  - Added `.meta/images` directory for workshop assets
- **README.md**: Enhanced compatibility section with additional recommended mods:
  - Added "A Super Spooky Song Pack" - adds spooky horror themes and song tracks
  - Added "Batong Vampire" - adds a race of Batong Vampires
  - Added "Express + Terramart HalloWeen" - Halloween-themed store replacements
  - Added reference to this CHANGELOG.md file

---

## [1.0.0] - Initial Release

### Features

- Initial SpookySynergy mod release
- Base Halloween-themed content integration
- Recipe patches for various crafting stations
- Treasure pool modifications for Halloween rewards
- Compatibility patches for multiple Halloween mods
