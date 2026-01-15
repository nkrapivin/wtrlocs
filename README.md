# We. The Revolution extended localizations

This repository contains open data for new localizations of [We. The Revolution](https://store.steampowered.com/app/736850/We_The_Revolution)

These languages can only be loaded by new builds of the game produced by us (Valkyrie Initiative)

The text is stored in the exact same format as it was originally stored by the developers of this game (it seems so).

## Testing

- Install the newest build of We. The Revolution that supports `vilangs` (currently - this is only the playtest builds)
- Clone this Git repository somewhere outside the game folder
- Replace the `vilangs` folder in `<Game folder>\We.TheRevolution_x86_64_Data\StreamingAssets` to the folder from this repository
- Launch the game through Steam
- Observe the changes

## Getting the original localizations

- There are two ways:
- See the `original` folder in this repository (changes to it are NOT accepted for obvious reasons, this isn't our text)
- Run the playtest build with the `-vidumporiginallanguages` launch parameter, and the original languages will be dumped to the `_dump` folder in your PersistentDataPath (IDs 0 to 3)

## Submitting your changes

- Make your changes to txt files in the cloned repository
- Submit a PR (please also tell us how to credit you)
- We will review the PR, provide any commentary, reject/accept
- If your PR is accepted, we will tell you through PR comments when/if your changes are live
- For legal reasons, please, keep in mind that by submitting your changes, you transfer the rights to your changes to us
- We will try our best to credit you, but keep in mind that legally, we have absolute rights over all files in the `vilangs` folder

## Technical stuff

`name.txt` contains the name of the language as it should be displayed in the settings menu. **Do not edit unless necessary.**

`steamcode.txt` must contain only the Steamworks SDK language code of the language, for English this is `english`, for Simplified Chinese this is `schinese`. This is necessary for Steam language detection. Do not edit unless necessary.

`vicredits.txt` contains the english-only text version of credits that can be opened in the main menu.

`vilangsrevision.txt` (Steam build only!) contains a link to the commit of the bundled translation data.

The game is made with Unity, so whenever you see angular `<...>` brackets, those are Unity text formatting tags, and when you see curly brackets `{0} {1}`, those are C# string formatting symbols. Please try to preserve them when making your edits.

Please also preserve the original line endings of any files you edit.

IDs 0 to 3 are reserved for the four original languages and must not be used.

- ID 4: German
- ID 5: Simplified Chinese
- ID 6: Spanish
- ID 7: Korean
- ID 8: Brazilian portuguese
- ID 9: Japanese
- ID 10: Turkish

