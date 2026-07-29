# minui-search-pak (RG35XX Plus/H/SP Fork)

An app for searching your ROM collection under the custom MinUI launcher.

This is a fork of [tanbase/minui-search-pak](https://github.com/tanbase/minui-search-pak) (originally developed by [laesetuc](https://github.com/laesetuc)) that adds support for the Anbernic H700-based devices (`rg35xxplus` platform).

## Requirements

This pak is designed for and tested with the following MinUI platforms and devices:

- `rg35xxplus`: Anbernic RG35XX Plus, RG35XX H, and RG35XX SP
- `tg5040`: Trimui Brick (formerly `tg3040`)

## Changes in this Fork

- **Added `rg35xxplus` Platform Binaries**: Included pre-compiled 32-bit ARM binaries of the UI components (`minui-keyboard`, `minui-list`, and `minui-presenter`) specifically built for the RG35XX Plus/H/SP toolchain.
- **Config Updates**: Updated `config.json` and `pak.json` to register the `rg35xxplus` platform.

## Installation

1. Mount your MinUI SD card.
2. Clone this repository or download the package files.
3. Copy the `Search.pak` directory to the platform folder in the `/Tools` directory on your SD card.
   - For Anbernic RG35XX SP/Plus/H: `/Tools/rg35xxplus/Search.pak/`
   - For Trimui Brick: `/Tools/tg5040/Search.pak/`
4. Confirm that the structure matches: `/Tools/$PLATFORM/Search.pak/launch.sh`
5. Unmount your SD Card and insert it into your MinUI device.

## Usage

1. Put the card into the TF1 slot of your Anbernic RG35XXSP.
2. Power on the device.
3. Navigate to **Tools** -> **Search**.
4. Enter your search query using the virtual keyboard.

### Search

Use the keyboard to enter a search term.  

- **A**: Select a character.
- **B**: Erase a character.
- **X**: Search.
- **Y**: Exit.

### Search Results

- Matching search results will be displayed in a list.
- Select a game and press A to launch the game, or B to return to the Search screen.

### Previous Search

When launching search again, the previous search results will be displayed.

## Acknowledgements & Third-Party Attribution

- **Original Project**: [minui-search-pak](https://github.com/tanbase/minui-search-pak) by [laesetuc](https://github.com/laesetuc) ([tanbase](https://github.com/tanbase))
- **MinUI Launcher**: [MinUI](https://github.com/shauninman/MinUI) by [Shaun Inman](https://github.com/shauninman)
- **Platform Binaries**:
  - The `rg35xxplus` binaries (`minui-keyboard`, `minui-list`, and `minui-presenter`) are sourced from the official releases of [Jose Diaz-Gonzalez](https://github.com/josegonzalez)'s repositories:
    - [minui-keyboard](https://github.com/josegonzalez/minui-keyboard) (v0.8.0)
    - [minui-list](https://github.com/josegonzalez/minui-list) (v0.14.0)
    - [minui-presenter](https://github.com/josegonzalez/minui-presenter) (v0.12.0)
  - Also, thank you, [Jose Diaz-Gonzalez](https://github.com/josegonzalez), for your pak repositories, which this project is based on.

## License

This project is released under the MIT License. For more information, see the [LICENSE](LICENSE) file.
