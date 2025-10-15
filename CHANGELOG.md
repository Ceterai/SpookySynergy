# Changelog

All notable changes to this project will be documented in this file.

The format is loosely based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.2a] - The Harrowing Patch Update

- **Patch Update**: Fixed a minor issue in `thea-events.treasurepools.patch` where an extra comma was present, which could cause JSON parsing errors in some cases. This update ensures compatibility and proper functionality of the patch.

## [1.0.2] - The Harrowing

### Added in 1.0.2

- **Harrowing Event Integration** (Elithian Races Mod support):
  - Released a separate patch mod for Harrowing event integration: [SpookySynergy - The Harrowing](https://steamcommunity.com/sharedfiles/filedetails/?id=3586407233)
  - As a basic improvement (if you don't want to install the patch mentioned above):
    - Added `harrowingcache.activeitem.patch` to balance Harrowing Cache similarly to the Haunted Bag and to teach new Harrowing crafting recipes
    - Added treasure pool patch (`thea-events.treasurepools.patch`) to enhance Harrowing Cache loot with flasks, cosmetics and candy from the Haunted Bag loot
    - Added patches for 6 Harrowing Candy variants (`harrowingcandyaqua`, `harrowingcandyblue`, `harrowingcandygreen`, `harrowingcandyorange`, `harrowingcandypink`, `harrowingcandyyellow`) to teach candy bowl crafting recipe on pickup, making them consistent with other mod candies
    - Added patches for Harrowing decorative objects:
      - `harrowingbannerlong.object.patch` - Long Harrowing banner colony tag expansion
      - `harrowingbannershort.object.patch` - Short Harrowing banner colony tag expansion
      - `harrowingpumpkin.object.patch` - Harrowing pumpkin colony tag expansion

- **Tabula Rasa Integration**:
  - Added `"spookysynergy"` group to all recipe files and patches for proper integration with Tabula Rasa
  - Added custom filter button for SpookySynergy recipes in Tabula Rasa crafting interface
    - Includes custom filter icons (`spookysynergy.png`, `spookysynergy_selected.png`)
    - Enables easy access to all SpookySynergy recipes through Tabula Rasa mod

- **Gothic Furniture Integration**:
  - Added recipes for 6 Gothic furniture items to make them craftable in the Haunted Crafting Table.

- **Wardrobe Interface & Spawnable Item Pack Support**:
  - Added support for Wardrobe Interface mod:
    - Created `wardrobe/spookysynergy.json` to add SpookySynergy items to Wardrobe Interface
  - Added support for Spawnable Item Pack mod:
    - Created `sipMods/spookysynergy.json` to add SpookySynergy items to Spawnable Item Pack

- **Equivalent Exchange & Improved Food Descriptions & Craftable Seeds Support**:
  - Added `EES_transmutationstudylist.config.patch` to include pumpkins in Equivalent Exchange transmutation study list
  - Added `IFD_fooddescription.patch` to add effect names of Halloween effects to food descriptions for Improved Food Descriptions mod
  - Added recipes for pumpkin and turnip seeds to be compatible with Craftable Seeds mod

### Changed in 1.0.2

- **Enhanced Item Integration**:
  - Updated Jack-O-Lanterns accross multiple mods to use the same sounds as the Jack-O-Lanterns from Nazar's Halloween
  - Updated Haunted Bag active item patch to match Harrowing Cache item
  - Rebalanced candy taking into account Harrowing Candy

### Technical Improvements in 1.0.2

- **README.md**: Updated documentation with latest mod features and compatibility information
- **Standardization**: Refactored existing patches and recipes for consistency

---

## [1.0.1] - Haunted Bag Enhancement

### Added in 1.0.1

- **Halloween mask patches**: Updates for rarity and pricing:
  - Patched 5 new Halloween mask variants (`hallowmask1-5`)
  - Patched 5 new Phobe mask variants (`phobemask1-5`)
  - Patched 3 new pumpkin head variants (`halhumanoidpump`, `halhylotlpump`, `halpumpkinhead`)

### Changed in 1.0.1

- **Halloween Reward Treasure Pools**: Rebalanced item drop weights and fixed item parameters syntax:
  - Adjusted pool round probabilities: changed from [0.5, 0]/[0.5, 1] to [0.4, 0]/[0.6, 1]
  - Reduced Phobe mask weights from 0.2 to 0.15 each for better balance
  - Reduced pumpkin head weights from 0.1 to 0.08 each
  - Fixed item syntax for colored items: converted from `"parameters"` format to array format `[item, count, parameters]`
    - Fixed wizard hat color variants
    - Fixed monster head color variants (eye, mushroom, creeper, yeti, eyeball, lagoon, slime heads)
    - Fixed pirate head color variant

### Technical Improvements in 1.0.1

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
