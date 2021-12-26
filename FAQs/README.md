# Common Modding Setup Errors
Anyone can contribute to this project by creating a pull request.

## Required for modding
_**Please**_ read [this](https://discord.com/channels/676880716142739467/799404622682390599/888912974088114186) before you do any modding!

## Packing/Unpacking
- If your .pak file is a few bytes or completely empty then it has not packed your files. Check you have used the tool correctly.
- REMEMBER to put your Content folder INSIDE of the Input folder!

## Locally loading your mod for testing
- Two methods:
    - "steamapps\common\Deep Rock Galactic\FSD\Content\Paks" - you **must** end the pak filename with "_P" in order for the game to load it e.g. new _P.pak
        - Mods in the Paks folder will show up as "Deprecated" in the mods list but will still work
    - "steamapps\common\Deep Rock Galactic\FSD\Content\Mods\your mod name" - additionally, if your mod is a BP mod, it **must** go into this folder for local testing

## Editing uasset and uexp files
Both files can be open directly with a hex editor, or edited with the recommended tools UassetGUI and DAUM. Both of these require you to select/open the uasset file, but will **also** affect the corresponding **uexp** file.
In UassetGUI you will see the uexp part of the files under the Export Data tab.

## Fully resetting your mods
1. Open drg.mod.io in a web browser and unsubscribe from all mods.
2. Run DRG and they should all uninstall.
3. Repeat if any mods exist (as possible).
4. Close DRG and delete the following folders: C:\Users\Public\mod.io\2475 and C:\Users[your username]\AppData\Local\mod.io
5. Run DRG and begin installing mods with modio as normal.

## Useful information regarding mod support
1. [Mod support FAQ](https://www.deeprockgalactic.com/modding-support-faq)
2. [Approval process](https://drg.mod.io/guides/approval-process-and-checklist-for-upload)
3. [Mod support announcement](https://steamcommunity.com/games/DeepRockGalactic/announcements/detail/2953787944888179529)

## UE4 Directory structure
To learn more about the folders in your UE4 project, visit https://docs.unrealengine.com/4.27/en-US/Basics/DirectoryStructure/
