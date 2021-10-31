# Character Template
This is a template for if you want to try and make a custom H3VR character using YAML.

This doesn't make Take & Hold Tweaker use YAML so much as it does automatically convert YAML files to JSON.

## Instructions:
1. Download this repository and open it in [Visual Studio Code](https://code.visualstudio.com/).
  [GitHub Desktop]() gives you the option to open the repository in VSC from it, and it makes handling a bunch of things easier, I'd recommend using it or a similar alternative.
2. Make sure to install the recommended extensions, this won't work properly without them.
3. Download [YQ](https://github.com/mikefarah/yq/releases), I'm assuming anyone following this is on Windows, you'll likely be after the *yq_windows_amd64.exe* file, just grab that and plonk it in the repository, it will not be uploaded to GitHub if you plan on uploading the character itself.

That should be enough to get started!

## Notes:
- For better and for worse, this is actually a rather aggressive setup, it will automatically convert any YAML or JSON file to the other when you save it regardless of where it is on your PC when you save it in Visual Studio Code *as long as* this folder is open in the program.
- This repository is automatically set up for development for Thunderstore and it's associated mod managers, you can zip up the folders and files inside the Release/ folder, upload them to Thunderstore and bang, mod should work just fine.
- Sosig files can be added into the sosig folder and vault files into the vault folder, these will automatically be detected and work with the custom character as long as they have the prefix "sosig_" or "vault_" respectively.
- If you want to have your character files automatically added to the game, go into R2ModMan's settings and find where the files are, go to BepInEx > Plugins and copy the file path to it, then open the command line (you can just type CMD into the Windows 10 search bar), type `mklink /J "[press ctrl+v]\[new folder name]" "[template repository path]\Release\plugins\CharacterTemplate"` (or whatever you've renamed CharacterTemplate to) into the window and press enter, those two folders have now formed a blood pact and are eternally bound together, or in other words, these two folders will always have the exact same thing inside.
- Make sure to edit both manifest.json files to be more accurate to the character you're making, and replace the icon.png and thumb.png files... Unless you like the errors.

## Credit:
This weird, horrendous, wonky mess wouldn't be possible without [AshHat](https://github.com/ash-hat/), it would likely be better set-up how it is now but they created the foundation I haphazardly built upon to bring this terribleness to you.