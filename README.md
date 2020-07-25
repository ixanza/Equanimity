# Equanimity

- [Equanimity](#equanimity)
  - [Preamble](#preamble)
  - [Installation](#installation)
    - [Pre-Installation](#pre-installation)
      - [Installing Microsoft Visual C++ Redistributable Package](#installing-microsoft-visual-c-redistributable-package)
      - [Steam Config](#steam-config)
        - [Disable the Steam Overlay](#disable-the-steam-overlay)
      - [Change Steams Update Behavior](#change-steams-update-behavior)
      - [Set the Game language to English](#set-the-game-language-to-english)
      - [Clean Skyrim](#clean-skyrim)
      - [Start Skyrim](#start-skyrim)
    - [Using Wabbajack](#using-wabbajack)
      - [Preparations](#preparations)
      - [Downloading and Installing](#downloading-and-installing)
        - [Problems with Wabbajack](#problems-with-wabbajack)
    - [Post-Installation](#post-installation)
      - [Copy Game Folder Files](#copy-game-folder-files)
      - [Getting an ENB](#getting-an-enb)
        - [Note : Please check that vsync is set to disable in enblocal.ini otherwise you will be stuck compiling shaders](#note--please-check-that-vsync-is-set-to-disable-in-enblocalini-otherwise-you-will-be-stuck-compiling-shaders)
  - [How to start up Equanimity](#how-to-start-up-equanimity)
  - [Updating](#updating)
  - [Creating your Character](#creating-your-character)
  - [In-Game MCM Options](#in-game-mcm-options)
    - [A Matter of Time](#a-matter-of-time)
    - [Follower Framework](#follower-framework)
    - [Honed Metal](#honed-metal)
    - [LOTD Settings](#lotd-settings)
    - [Quick Light](#quick-light)
    - [SkyUI](#skyui)
    - [VioLens](#violens)
  - [FAQ](#faq)
    - [Ultrawide Options](#ultrawide-options)
    - [Tweaking the Game Settings](#tweaking-the-game-settings)
  - [Removing the Modlist](#removing-the-modlist)
  - [Credits and Thanks](#credits-and-thanks)
  - [Contact](#contact)
  - [Contributing](#contributing)
  - [Changelog](#changelog)

## Preamble

Equanimity is a list focusing on a different style of gameplay. It consists of multiple mods enhancing different aspects of the game for a unique feel. Equanimity uses mods such as: 
- Adamant and Mysticism for perks and magic
- Combat Gameplay Overhaul, Wildcat, Ultimate Combat for combat
- OMEGA Updated, KS Dragon Overhaul for encounter levels and zones
- True Unleveled Skyrim to distribute perks to enemies
- SkyREM RaE for races
- Curse of the Firmament for standing stones
- Better Vampires and Growl for vampirism  and lycantrophy respectively

Equanimity comes with a list of land expansions and quest expansions such as :
- Legacy of the Dragonborn
- Interesting NPCS
- Vigilant
- Wyrmstooth
- Wheels of Lull
- Helgen Reborn
- Project AHO

## Installation

### Pre-Installation

These steps are only needed if you install this Modlist for the first time. If you update the Modlist, jump straight to [Updating](#updating).

#### Installing Microsoft Visual C++ Redistributable Package

I doubt you need to do this since you likely already have this installed. The package is required for MO2 and you can download it from [Microsoft](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads). Download the x64 version under "Visual Studio 2015, 2017 and 2019". [Direct link](https://aka.ms/vs/16/release/vc_redist.x64.exe) if you can't find it.

#### Steam Config

##### Disable the Steam Overlay

The Steam Overlay can cause issues with ENB and is recommended to be turned off.

Open the Properties window (right click the game in your Library->Properties), navigate to the _General_ tab and un-tick the _Enable the Steam Overlay while in-game_ checkbox.

#### Change Steams Update Behavior

SSE is still being updated by Bethesda (they only add Creation Club content). Whenever the game updates, the entire modding community goes silent for the next one or two weeks because some mods need to be updated to the latest game runtime version.

To ensure that Steam does not automatically updates the game for you, head over to the Properties window, navigate to the _Updates_ tab and change _Automatic updates_ to _Only update this game when I launch it_. You should also disable the Steam Cloud while you're at it.

#### Set the Game language to English

Just do it. This entire Modlist is in English and 99% of all mods you will find are also in English. I highly recommend playing the game in English and **I will not give support to people with a non-English game**.

Open the Steam Properties window, navigate to the _Language_ tab and select _English_ from the dropdown menu.

#### Clean Skyrim

I highly recommend uninstalling the game through Steam, deleting the game folder and reinstalling it. You should also clean up the `Skyrim Special Edition` folder in `Documents/My Games/` by deleting the contents in it.

#### Start Skyrim

After you have done everything above and got a clean SSE installation ready, start the Launcher and and let it do the initial graphics check. Do not worry about this part as the installation will replace this graphics settings.
Start the game and exit once you're in the main menu.

### Using Wabbajack

#### Preparations

Grab the latest release of Wabbajack from [here](https://github.com/wabbajack-tools/wabbajack/releases) and place the `Wabbajack.exe` file in a _working folder_. This folder **must not** be in a _common folders_ like your Desktop, Downloads or Program Files folder. It's best to create a Wabbajack folder near the root level of your drive like `C:/Wabbajack`.

Head to [releases](https://github.com/ixanza/Equanimity/releases) and grab the latest .wabbajack file from there. Once downloaded double click the .wabbajack file to open up the installer. Set the Installation folder to somewhere that is not affected by UAC (Please do not put it in Documents, Program Files, Desktop. Put it somewhere easy like `C:/Modlists/Equanimity`). The downloads path should automatically fill in the installation path.

#### Downloading and Installing

The download and installation process can take a very long time depending on your system specs. Wabbajack will calculate the amount of threads it will use at the start of the installation. To have the highest amount of threads and thus the fastest speed, it is advised to have the working folder on an SSD.

1. Open Wabbajack
2. Load the Modlist from Disk
3. Adjust the download and installation paths
4. Click the Go/Begin button
5. Wait for Wabbajack to finish

##### Problems with Wabbajack

There are a lot of different scenarios where Wabbajack will produce an error. I recommend re-running Wabbajack before posting anything. Wabbajack will continue where it left off so you loose no progress.

**Could not download x**:

If a mod updated and the old files got deleted, it is impossible to download them. In this case just wait till I update the Modlist.

**x is not a whitelisted download**:

This can happen when I update the modlist. Check if a new update is available and wait if there is none.

**Wabbajack could not find my game folder**:

Wabbajack will not work with a pirated version of the game. If you own the game on Steam, go back to the [Pre-Installation](#pre-installation) step.

### Post-Installation

#### Copy Game Folder Files

Download the latest ENB Series from [here](http://enbdev.com/download_mod_tesskyrimse.htm) and copy `d3d11.dll` and `d3dcompiler_46e.dll` to your game folder.

Copy the all of the files from the `MO2/Game Folder Files` directory into your game folder.

#### Getting an ENB

This list uses Obsidian Weathers Weathers so you want to get an ENB that is compatible.

Once you found a preset you like. Download it and extract the enbseries folder, enbseries.ini and enblocal.ini to your Skyrim Special Edition directory.

##### Note : Please check that vsync is set to disable in enblocal.ini otherwise you will be stuck compiling shaders

## How to start up Equanimity

Head over to the installation folder and locate an executable named `ModOrganizer.exe` and launch it. Once its launched there will be a dropdown box on the top right and a big run button next to it. Ensure it is set to SKSE by selecting it in the dropdown box and then hitting the run button.

## Updating

If this Modlist receives an update please check the Changelog before doing anything. Always backup your saves or start a new game after updating.

**Wabbajack will delete all files that are not part of the Modlist when updating!**

This means that any additional mods you have installed on top of the Modlist will be deleted. Your downloads folder will not be touched!

Updating is like installing. You only have to make sure that you select the same path and tick the _overwrite existing Modlist_ button.

## Creating your Character

Upon entering the game you will be greeted with a notification from the Relic Notifications Mod. Hit OK and wait for another pop-up from it, usually takes about a minute.  Once it's done you can proceed with creating your character. Once you've named your character wait for all the messages in the top left to fade away then open your inventory and close it. This will start up Requiem. Once Requiem has finished its installation you may proceed with the next section. While creating your character you may receive a pop up asking you if you want to scan now or later from Relic Notifications. Hit scan now to proceed.

## In-Game MCM Options

Once the game has loaded. Wait until there are no more messages on the top left corner. Then you can hit escape and click on Mod Configuration to continue this section.
Mods with (Preference) next to their name is solely preferential and do not affect the balance of the game.

### A Matter of Time (Preference)

- Presets :
  - Load user settings

### Better Vampires

- Hotkeys :
  - Set these up as you like. I personally only put nightvision on H
- General Options :
  - Rank Progression : Normal - Necks Bitten
  - Stage Hated : Stage 4 Hated
  - Feeding Animation : Bedroll feeding Animation
  - Sun Damage : Slight Damage
  - Specialised Sun Damage : Exempt at Stage 1
- Miscellaneous Options :
  - Abilities have Recharge Timers : Tick
  - Vampire Drain will affect Satiation : Tick
  - Enthralled Victims Change Clothing : Untick
  
### Complete Crafting

- Recipe Display → Crafting Menu Filters :
  - Breakdown Recipes - Tick
- Recipe Display → Additional Display Options :
  - Craft Daedric Items Only at Night: Tick
- Crafting Options → Additional Items :
  - Artifact Replicas : Tick
  - Matching Set Circlets : Tick
- Learning & XP → Smithing Experience :
  - Tanning Rack : 0.1
  - Smelter : 0.1
 Mining  and Materials → Mining :
  - Mining Presets : FASTER MINING
- Mining  and Materials → Firewood :
  - Firewood per chop : 6
  - Max per activation : 1
- Tempering and Enchanting → Variable Tempering Strength : 
  - Enable Tempering Adjustments : Tick
- Tempering and Enchanting → Variable Enchantment Strength : 
  - Enable Enchanting Adjustments : Tick

### CGO

- Unlocked Grip :
  - Hotkey : (Preference)
  - NPCs Change Grip : Unticked
- Dodge Roll :
  - NPCs Dodge : Unticked
- Leaning (Preference) : 
  - Lean Multiplier (1st Person) : X0.5
  - Lean Multiplier (3rd Person) : X0.5
- Camera Noise (Preference) :
  - Camera Noise Mult (1st Person) : X0.0
- Dual Wield Blocking :
  - Hotkey : (Preference)

### Enhanced Blood (Preference)
- Screen Blood:
  - Enabled : Untick

### Extended UI (Preference)
- Stats Menu
  - Hide Legendary UI Elements - Tick
  - Show attribute modifiers - Tick
  - Show skill modifiers - Tick
- Console
  - Fullscreen : Tick

### Follower Framework

- System → Save/Load Configuration :
  - Load from File : Click

### Honed Metal

- General :
  - Crafting Cost Multiplier : 0.85
  - Tempering Cost Multiplier : 0.35
  - Enchanting Cost Multiplier : 0.75
  - Recharge Cost Multiplier : 0.85
  - Materials Cost Multiplier : 1.10
- Maintenance :
  - Crafting Time : 0.5
  - Enchanting Time : 0.5
  - Recharging Time : 0.0
  - Common Materials Acquisition Time : 0.02

### Immersive HUD (Preference)

- Set this up however you like. There are some default options already tweaked

### KS Dragon Overhaul 2
- Toggle Mod : Tick
- Combat →  Kill Move Settings 
  - Use Modified : Tick
- Combat → Other Settings
  - Recoil/Physical Effect : Tick
  - Timed Stagger : Tick
- Difficulty → Preset List
  - List : Slightly

### LOTD Settings

- LOTD Settings → General → Shippment Crate Locations :
  - Carriages : Enabled
  - Inns : Enabled
  - Player Houses : Enabled

### LOTD : The Curator's Tracker (Preference)
- Settings → Mod Settings : 
  - Live Another Life Config : Pick according to the start you decide
  - Helgen Reborn Config : Pick according to whichever option you choose in the quest. You don't have to do it now

### Lucien (Preference)

- If you use a player name thats in this selection, Lucien will call you by this name

### MoreHUD (Preference)

- Set this up however you like. There are some default options alredy tweaked

### Quick Light

- Quick Light → Brightness :
  - Brightness - Bright

### SkyUI

- General → Item List :
  - Font Size : Small
  - Category Icon Theme : CELTIC

### Timing is Everything (Preference)

- Set this up however you like or load a pre-configured preset
- Note if loading the pre-configured preset to follow the steps below
- Extra Options → Presets
  - Load Preset
- Then cycle through DLC Quests, Other Quests, and Extra options again and load the preset a second time

### Ultimate Combat

- General → Timed Block : 
  - Effective Time : 0.00s
  - Blur Strength : 0.0s
- General → Game Balance Settings : 
  - Speed Bonus : Disabled
- General → Others :
  - Swing Effect : Disabled
- General → Stagger : 
  - Enemy Pose : Disabled
  - Player Stagger : Disabled
  - NPC's Bow Poise : 0.00s
  - Player Bow Poise : 0.00s
- General → Locational : 
  - Headshot Damage Mult : 0.0
  - Headshot Message : Disabled
  - Locational Damage Sound : Disabled
  - Locational Damage Effect : Disabled
- NPC Settings → Giant : 
  - Max HP Scale : Max HP 1.0
- NPC Settings → Dwarven Centurion : 
  - HP Mult : HP 1.0
- NPC Settings → Dragon Priest : 
  - HP Mult : HP 1.0

### VioLens

- Profile System → Menu Settings :
  - Load : VIOLENS CONFIG

## FAQ

### Ultrawide Options

If you have an ultrawide monitor (21:9), the UI will be off. You will want to reinstall Dear Diary with the widescreen option. Pick any options on the FOMOD you want but ensure Extended UI, More Informative Console and Morehud is ticked

### Tweaking the Game Settings

I highly recommend using [BethINI](https://www.nexusmods.com/skyrimspecialedition/mods/4875) which is included in this Modlist (can be found in `MO2/tools/BethINI`). I recommend tweaking the `Detail` section for more FPS:

- `Shadow Resolution`: Very big one. A good balance is `2048` which is the borderline between high FPS drainage and garbage looking shadows.
- `Ambient Occlusion`: Highly recommended to turn either this or your ENB version off. Do not have the game AO and an ENB AO turned on at the same time.
- `Remove Shadows`: If you really struggle, use this. This will disable all Shadows (not recommended)

## Removing the Modlist

You can just remove the MO2 folder and be done with it. SKSE and ENB files will still be in your game folder so I recommend using [ENB and ReShade Manager](https://www.nexusmods.com/skyrimspecialedition/mods/4143) if you want to remove the ENB.

## Credits and Thanks

- _YOU_ for actually reading the readme. Thanks a ton!!
- Total, jdsmith2816, SirJesto for helping me out with a lot of the conflict resolution
- erri120 & jdsmith2816 - Repository template
- Halgari and everyone the WJ Team - Wabbajack is awesome and so are you

## Contact

While I'm always available on the [Wabbajack Discord](https://discord.gg/wabbajack), I would advise checking the [Issues](https://github.com/ixanza/equanimity/issues) (open **and** closed ones) on GitHub first if you have any problems. The same goes for _Enhancements_ or _Feature/Mod Requests_. **DO NOT DM ME ON DISCORD. I WILL NOT PROVIDE SUPPORT FOR YOU IN DMS AND I WILL BLOCK YOU**.

## Contributing

See [Contributing](CONTRIBUTING.md).

## Changelog

See [Changelog](CHANGELOG.md).
