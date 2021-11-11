# Common Modding Setup Errors
Anyone can contribute to this project by creating a pull request.

### Packing/Unpacking
- UE version needs to be 4.25.xx
- Paths in the input.txt and pack.bat/unpack.bat need enclosing "" for any paths containing spaces
- In the input.txt there should be a '\' after input -> "Path\DRGpacker\input<b>\</b>" "../../../FSD/"
- Common path example for the mod files would be "DRGpacker\input\\**Content**\WeaponsNTools"
- It is important to be consistent here so with the above input.txt, don’t skip neither "input" nor "Content" in the path to the mod files

### Locally loading your mod for testing
- Two methods:
    - "steamapps\common\Deep Rock Galactic\FSD\Content\Paks" - you **must** end the pak filename with "_P" in order for the game to load it e.g. new _P.pak
        - Mods in the Paks folder will show up as "Deprecated" in the mods list but will still work
    - "steamapps\common\Deep Rock Galactic\FSD\Content\Mods\your mod name" - additionally, if your mod is a BP mod, it **must** go into this folder for local testing