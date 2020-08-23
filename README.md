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
    - [ENB](#enb)
  - [Noteworthy Mods](#noteworthy-mods)
    - [Gameplay](#gameplay)
    - [Quest and Encounter Mods](#quest-and-encounter-mods)
    - [Expanded Cities Towns and Villages](#expanded-cities-towns-and-villages)
    - [NPC Retextures](#npc-retextures)
    - [Followers](#followers)
    - [Audio and Weather](#audio-and-weather)
    - [New Equippables](#new-equippables)
  - [How to start up Equanimity](#how-to-start-up-equanimity)
  - [Updating](#updating)
  - [Creating your Character](#creating-your-character)
  - [In-Game MCM Options](#in-game-mcm-options)
    - [Better Vampires](#better-vampires)
    - [Complete Crafting](#complete-crafting)
    - [CGO](#cgo)
    - [Trade and Barter](#trade-and-barter)
  - [Other Post Installation FAQ](#other-post-installation-faq)
    - [Ultrawide Options](#ultrawide-options)
    - [Tweaking the Game Settings](#tweaking-the-game-settings)
    - [Zoomed in Display](#zoomed-in-display)
    - [Removing the Modlist](#removing-the-modlist)
  - [Credits and Thanks](#credits-and-thanks)
  - [Contact](#contact)
  - [Contributing](#contributing)
  - [Changelog](#changelog)

## Preamble

Equanimity is a list focusing on a different style of gameplay based on the full Simonrim Suite with a lot of mod interaction to make the game feel very similar yet different. Check the [Noteworthy Mods](#noteworthy-mods) section later on for more information on what is provided.

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

#### Downloading and Installing

The download and installation process can take a very long time depending on your system specs. Wabbajack will calculate the amount of threads it will use at the start of the installation. To have the highest amount of threads and thus the fastest speed, it is advised to have the working folder on an SSD.

1. Open Wabbajack
2. Click on Browse Modlists, and download Equanimity from the gallery.
3. Once the download is done set the Installation folder to somewhere that is not affected by UAC (Please do not put it in Documents, Program Files, Desktop. Put it somewhere easy like `C:/Modlists/Equanimity`). The downloads path should automatically fill in the installation path.
4. Click the Go/Begin button
5. Wait for Wabbajack to finish
6. If you run into any issues see the next section. If the installation is successful, proceed to [Post-Installation](#post-installation).

##### Problems with Wabbajack

There are a lot of different scenarios where Wabbajack will produce an error. I recommend re-running Wabbajack before posting anything. Wabbajack will continue where it left off so you loose no progress.

**Could not download x**:

If a mod updated and the old files got deleted, it is impossible to download them. In this case just wait till I update the Modlist.

**x is not a whitelisted download**:

This can happen when I update the modlist. Check if a new update is available and wait if there is none.

**Wabbajack could not find my game folder**:

Wabbajack will not work with a pirated version of the game. If you own the game on Steam, go back to the [Pre-Installation](#pre-installation) step.

**Windows is reporting that a virus has been detected**:

Windows 10 has started to auto quarantine the usvfs_proxy_x86.exe file from the latest version of Mod Organizer 2 saying a threat was detected . This is a known false postive confirmed by the MO2 Devs. You can fix this by adding an exemption for MO2 Folder to your Antivirus. Example for windows defender can be found [here](https://www.thewindowsclub.com/exclude-a-folder-from-windows-security-scan).

## Post-Installation

### Copy Game Folder Files

Copy the all of the files from the `Installation Folder/Game Folder Files` directory into your game folder.

### ENB

Equanimity comes configured with [Ljoss](https://www.nexusmods.com/skyrimspecialedition/mods/30971)

If you want a different ENB. You can choose from a wide variety of ENBs on the Nexus that support Cathedral Weathers. To replace the ENB installed. Delete the enbcache folder, enbseries folder, enbseries.ini and replace those with the new ENB. You don't have to delete the enblocal.ini as that contains tweaks that don't affect how it looks but rather things like screenshot formats, vsync settings.

A few other ENB suggestions are:

- [Rudy ENB for Cathedral Weathers](https://www.nexusmods.com/skyrimspecialedition/mods/39113)
- [Silent Horizons](https://www.nexusmods.com/skyrimspecialedition/mods/21543)
- [Serio's ENB](https://www.nexusmods.com/skyrimspecialedition/mods/30506)
- [Soul Spectrum ENB](https://www.nexusmods.com/skyrimspecialedition/mods/29675)

**Note:**
Please check that vsync is set to disable in enblocal.ini otherwise you will either be stuck compiling shaders or a black screen, or the menu with no options.

## Noteworthy Mods

### Gameplay

Equanimity uses the full suite of Simon Magus's mods which are:

1. [Adamant - A Perk Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/30191)
2. [Mysticism - A Magic Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/27839)
3. [Arena - An Encounter Zone Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/33487)
4. [Blade and Blunt - A Combat Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/34549)
5. [Aetherius - A Race Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/26686)
6. [Mundus - A Standing Stone Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/33411)

Various other mods are used to flesh out all aspects of the game as well such as:

1. [Better Vampires](https://www.nexusmods.com/skyrimspecialedition/mods/1925) for overhauling Vampires
2. [Growl - Werebeasts of Skyrim](https://www.nexusmods.com/skyrimspecialedition/mods/31245) for overhauling Lycantrophy
3. [Triumvirate - Mage Archetypes](https://www.nexusmods.com/skyrimspecialedition/mods/39170) which adds new mage archetypes to the game
4. [Complete Crafting Overhaul Remastered](https://www.nexusmods.com/skyrimspecialedition/mods/28608) which overhauls the crafting component of the game
5. [Skyrim Revamped - Complete Enemy Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/14598) which overhauls NPC and makes bosses harder
6. [Ultimate Combat](https://www.nexusmods.com/skyrimspecialedition/mods/17196) introduces new enemy AI which keeps the game fresh
7. [Combat Gameplay Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/33767) enables new combat mechanics such as jump attacks, unlocked grip and a dodge function
8. [Wintersun - Faiths of Skyrim](https://www.nexusmods.com/skyrimspecialedition/mods/22506) adds a religion aspect to the game in the form of worshipping aedras or daedras and getting rewarded for it

### Quest and Encounter Mods

Equanimity comes with a wide variety of new quest and encounters. A few are listed below.

[Legacy of the Dragonborn](https://www.nexusmods.com/skyrimspecialedition/mods/11802) is a very large mod that shapes the way how you play the game. The museum is a very robust house mod with the ability to display almost every item in the game and also has an extensive mod support which is utilised to some extent in Equanimity.

[Interesting NPCs](https://www.nexusmods.com/skyrimspecialedition/mods/29194) adds over 250 fully voiced NPCs, 25+ followers, 15+ marriage candidates and 50+ quests to fully flesh out the world of Skyrim. Every hold will feel more lively with more NPCs walking and talking with each other

[Missives](https://www.nexusmods.com/skyrimspecialedition/mods/17576?tab=files) adds a large number of localized radiant quests found at Missive Boards of varying difficulty and with varying rewards. Missives has been extended to Solstheim as well as Wyrmstooth.

[Vigilant](https://www.nexusmods.com/skyrimspecialedition/mods/11849) adds a whole new set of quests, enemies, equipment to the game revolving around the Vigilants of Stendar and Daedra. It has also been patched to work well with Requiem. For a good time you want to be atleast level 30 before attempting this.

[Wyrmstooth](https://archive.org/details/wyrmstooth1.18SSE) adds a new world and a series of quests involving killing a dragon for a bounty. It's a very well done quest mod.

[Helgen Reborn](https://www.nexusmods.com/skyrimspecialedition/mods/5673) adds a lengthy questline with the aim of rebuilding Helgen.

[Forgotten City](https://www.nexusmods.com/skyrimspecialedition/mods/1179) is a really good choice driven quest mod with a lot of endings surrounding the disappearance of a civilisation.

[Project AHO](https://www.nexusmods.com/skyrimspecialedition/mods/15996) is a medium sized DLC questline surroudning the Great House Telvanni.

[Undeath](https://www.nexusmods.com/skyrimspecialedition/mods/6180) is a quest and expansion mod that delves deep into necromancy and offers a new lich transformation.

[Wheels of Lull](https://www.nexusmods.com/skyrimspecialedition/mods/748) is an expansive questline filled with puzzles, infiltration, poltergeists, mad science, and butter.

Equanimity also has a lot of modified vanilla quests such as:

1. [Save the Icerunner - Lights Out Alternate Route](https://www.nexusmods.com/skyrimspecialedition/mods/34681)
2. [Finding Deerkethus](https://www.nexusmods.com/skyrimspecialedition/mods/19550)
3. [Finding Helgi and Laelette](https://www.nexusmods.com/skyrimspecialedition/mods/28973)
4. [Finding Velehk Sain](https://www.nexusmods.com/skyrimspecialedition/mods/19815)

### Expanded Cities Towns and Villages

Equanimity uses the full suite of [JK's Skyrim](https://www.nexusmods.com/skyrimspecialedition/mods/6289) along with all of the interior patches for it.

### NPC Retextures

I have to give credits to Darkladylexy from the popular [Lexy's Legacy of the Dragonborn Special Edition](https://lexyslotd.com) guide for her extremely well done choices of NPC mods. It is a combination of a lot of NPC mods with carefully picking which npc comes from which mod itself. For an overview of every single NPC that is retextured. Please see [this section on her guide](https://lexyslotd.com/guide/npc-retextures-page/)

The NPC retextures are largely in this order except a select few NPCs

1. WICO - Windsong Immersive Character Overhaul
2. Followers Hirelings and Housecarls
3. Metalsabers Beautiful Orcs of Skyrim
4. The Ordinary Women
5. Pandorable's NPCs
6. Kalilies NPCs
7. Fresh Faces
8. Pandorable's NPCs - Dawnguard
9. Pandorable's NPCs - Dragonborn
10. Bijin Warmaidens
11. Bijin Wives
12. Bijin NPCs
13. Seranaholic
14. Valerica
15. eeekie's Enhanced NPCs
16. RS Children Overhaul
17. Cuyima Interesting NPCs
18. High Poly Inigo
19. Legacy of the Dragonborn NPC Overhaul

For an overview of every single NPC that is retextured. Please see [this section on her guide](https://lexyslotd.com/guide/npc-retextures-page/).

### Followers

[Inigo](https://www.nexusmods.com/skyrimspecialedition/mods/1461) is a fully voiced khajiit adventuring companion with over 7000 lines of unique dialogue - much of it about you. He'll level alongside you and avoid most traps. If you're sneaking he won't chatter and he'll whisper if you talk to him. He can run out of arrows. He's highly skilled in archery, one-handed, and sneak.

[Lucien](https://www.nexusmods.com/skyrimspecialedition/mods/20035) is a fully voiced Imperial follower with around 3000 lines of immersive, lore-friendly dialogue. Though he arrives in Skyrim as a cowardly scholar, he'll gradually gain strength and confidence by your side until he grows into a hero in his own right.

### Audio and Weather

[Audio Overhaul Skyrim](https://www.nexusmods.com/skyrimspecialedition/mods/12466) and [Immersive Sounds Compendium](https://www.nexusmods.com/skyrimspecialedition/mods/523) offer an amazing base for skyrim's ambiance and foley.

### New Equippables

[Amulets of Skyrim](https://www.nexusmods.com/skyrimspecialedition/mods/487) adds new amulets as well as the ability to turn standing stone/artifact effects into necklaces and rings.

[Cloaks of Skyrim](https://www.nexusmods.com/skyrimspecialedition/mods/6369) provides cloaks to various NPCs.

[Heavy Armory](https://www.nexusmods.com/skyrimspecialedition/mods/6308) adds around 100 new weapons into the game that is evenly distributed to all the enemies and NPCs.

[Common Clothes and Armors](https://www.nexusmods.com/skyrimspecialedition/mods/21305) adds more variety of common clothes to leveled lists.

[Guard Armor Replacer](https://www.nexusmods.com/skyrimspecialedition/mods/22671) adds new guard and stormcloak looks.

[New Legion](https://www.nexusmods.com/skyrimspecialedition/mods/30468) adds new looks to the imperials.

[Unplayable Faction Armor](https://www.nexusmods.com/skyrimspecialedition/mods/30051) adds new armor to alik'r and vigilants and other npc archetypes

[NordwarUA's Race Armor Expansion](https://www.nexusmods.com/skyrimspecialedition/mods/34585) adds new armor to races like orcs

[Nordic Wanderer](https://www.nexusmods.com/skyrimspecialedition/mods/7943) adds two new swords and a new armour set for male and females. There is full weight-slider support and the armour should be compatible with all body mods.

[Volkihar Knight - Vampire Armor](https://www.nexusmods.com/skyrimspecialedition/mods/4806) is a really cool Vampire armour set that can be crafted or found in the Volkihar Castle from progressing in the Dawnguard Questline

[Sithis Armor](https://www.nexusmods.com/skyrimspecialedition/mods/39080) is an incredible armor set. The addon [Sithis Armor - Mastercraft Version](https://www.nexusmods.com/skyrimspecialedition/mods/39209/) adds additional sets, makes it easier to craft as well as adding CCOR compatibility.

## How to start up Equanimity

Head over to the installation folder and locate an executable named `ModOrganizer.exe` and launch it. Once its launched there will be a dropdown box on the top right and a big run button next to it. Ensure it is set to SKSE by selecting it in the dropdown box and then hitting the run button.

## Updating

If this Modlist receives an update please check the Changelog before doing anything. Always backup your saves or start a new game after updating.

**Wabbajack will delete all files that are not part of the Modlist when updating!**

This means that any additional mods you have installed on top of the Modlist will be deleted. Your downloads folder will not be touched!

Updating is like installing. You only have to make sure that you select the same path and tick the _overwrite existing Modlist_ button.

## Creating your Character

Upon entering the game you will be greeted with a notification from the Curator's Companion. Hit OK and wait for another pop-up from it, usually takes about a minute. Wait until there are no more messages on the top left corner. Then you can hit escape and click on Mod Configuration to continue this section.

Mods or sections with (Preference) next to their name is solely preferential and do not affect the balance of the game.

## In-Game MCM Options

### Better Vampires

- Hotkeys (Preference):
  - Set these up as you like. I personally only put nightvision on H
- General Options:
  - Rank Progression: Normal - Necks Bitten
  - Stage Hated: Stage 4 Hated
  - Feeding Animation: Bedroll feeding Animation
  - Sun Damage: Slight Damage
  - Specialised Sun Damage: Exempt at Stage 1
- Miscellaneous Options:
  - Abilities have Recharge Timers: Enabled
  
### Complete Crafting

- Recipe Display → Crafting Menu Filters:
  - Breakdown Recipes - Enabled
- Recipe Display → Additional Display Options:
  - Craft Daedric Items Only at Night: Enabled
- Crafting Options → Additional Items:
  - Artifact Replicas: Enabled
  - Matching Set Circlets: Enabled
- Learning & XP → Smithing Experience:
  - Tanning Rack: 0.1
  - Smelter: 0.1
 Mining  and Materials → Mining:
  - Mining Presets: FASTER MINING
- Mining  and Materials → Firewood:
  - Firewood per chop: 6
  - Max per activation: 1
- Tempering and Enchanting → Variable Tempering Strength:
  - Enable Tempering Adjustments: Enabled
- Tempering and Enchanting → Variable Enchantment Strength:
  - Enable Enchanting Adjustments: Enabled

### CGO

- Unlocked Grip:
  - Hotkey: (Preference)
- Leaning (Preference):
  - Lean Multiplier (1st Person): X0.5
  - Lean Multiplier (3rd Person): X0.5
- Camera Noise (Preference):
  - Camera Noise Mult (1st Person): X0.0
- Dual Wield Blocking:
  - Hotkey: (Preference)

### Trade and Barter

- Barter Rates → Settings:
  - Modify Barter Settings: Enabled
  - Barter Rates → Preset:
  - Barter Rate: Medium

The rest of the required MCM options have been automated for you. Enjoy the game or tweak the following to your liking:

- Immersive HUD
- All Geared up Derivative
- SkyUI
- Lucien (If you set a nickname that's supported he can call you by that name)
- XP32 Skeleton Styles

## Other Post Installation FAQ

### Ultrawide Options

If you have an ultrawide monitor (21:9), the UI will be off. You will want to reinstall Dear Diary with the widescreen option. Pick any options on the FOMOD you want but ensure Extended UI, More Informative Console and Morehud is ticked.
You will also want to install the SkyHud - High Resolution Widescreen Fix from [here](https://www.nexusmods.com/skyrimspecialedition/mods/1778/?).

### Tweaking the Game Settings

I highly recommend using [BethINI](https://www.nexusmods.com/skyrimspecialedition/mods/4875) which is included in this Modlist (can be found in `MO2/tools/BethINI`). I recommend tweaking the `Detail` section for more FPS:

- `Shadow Resolution`: Very big one. A good balance is `2048` which is the borderline between high FPS drainage and garbage looking shadows.
- `Ambient Occlusion`: Highly recommended to turn either this or your ENB version off. Do not have the game AO and an ENB AO turned on at the same time.
- `Remove Shadows`: If you really struggle, use this. This will disable all Shadows (not recommended)

### Zoomed in Display

This can be caused by Window's Display Scaling feature. This usually is set to above 100% when using very large (32 inch++) sized monitors and TVs. There are two solutions to this

- Set the display scaling back to 100% in the Screen Resolution Settings for Windows
- Edit the mod SSE Display Tweaks.
  - Under `[Render]`
    - Set Fullscreen to `True`
    - Set Borderless to `False`

### Removing the Modlist

You can just remove the MO2 folder and be done with it. SKSE and ENB files will still be in your game folder so I recommend using [ENB and ReShade Manager](https://www.nexusmods.com/skyrimspecialedition/mods/4143) if you want to remove the ENB.

## Credits and Thanks

- _YOU_ for actually reading the readme. Thanks a ton!!
- jdsmith2816 - for incredible help with getting mods working/patches/navmesh help
- DarkladyLexy for her consistency patches which I have used and modified upon as well as her colleciton of NPC overhauls which look amazing
- erri120 & jdsmith2816 - Repository template
- Halgari and everyone the WJ Team - Wabbajack is awesome and so are you

## Contact

While I'm always available on the [Wabbajack Discord](https://discord.gg/wabbajack), I would advise checking the [Issues](https://github.com/ixanza/equanimity/issues) (open **and** closed ones) on GitHub first if you have any problems. The same goes for _Enhancements_ or _Feature/Mod Requests_. **DO NOT DM ME ON DISCORD. I WILL NOT PROVIDE SUPPORT FOR YOU IN DMS AND I WILL BLOCK YOU**.

## Contributing

See [Contributing](CONTRIBUTING.md).

## Changelog

See [Changelog](CHANGELOG.md).
