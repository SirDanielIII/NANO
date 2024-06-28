# Na, No OptiFine (NANO)

The definitive Fabric performance modpack that aims to eliminate the need for OptiFine, **FOREVER**.

#### `Modpack Revision: 3.1`

### Changelog from Revision 3.0:

<details>
<br>

**Dropped Modpack Support For:**

- 1.20.1, 1.20.2 & 1.20.4

**Other Changes**

* Added [TCDCommons API](https://modrinth.com/mod/Eldc1g37) as it is required for newer versions of [Better Statistics Screen](https://modrinth.com/mod/better-stats)
* Added [Colormatic](https://modrinth.com/mod/colormatic) & [Polytone](https://modrinth.com/mod/polytone) to support OptiFine's custom colours (color.properties).
* Moved [Remove Reloading Screen](https://modrinth.com/mod/rrls) to [[Utility]](#utility)
* Moved [LambdaControls](https://modrinth.com/mod/lambdacontrols) & [MidnightControls](https://modrinth.com/mod/midnightcontrols) to [[Extra Features]](#extra-features)

</details>

## What is [OptiFine](https://www.optifine.net/home) & [Sodium](https://modrinth.com/mod/sodium)?

<details>
OptiFine is a very popular optimization mod that helps improve Minecraft's performance, and adds extra features that the vanilla client doesn't have. However, even while being a
performance mod, it's still very sluggish.

* E.G. Booting up the game or even changing resource packs takes foreverrrrrr...

Furthermore, the closed-source nature and intrusive characteristics of OptiFine pose challenges for other developers aiming to produce mods that are compatible with it.

Sodium is the free & open-source alternative to OptiFine that actually has **better performance**, and is compatible with a wide range of the Fabric mod ecosystem.
However, by itself, it lacks many of the beloved features from OptiFine, such as a zoom key, shader support, dynamic lighting, extreme customization with resource packs, etc.,
which can make transitioning out of OptiFine very difficult.
</details>

## So What Does This Modpack Do?

By using [the following mods](#mod-list), we're able to incorporate ALL of OptiFine's features, while still using Sodium! In addition, there are many quality of life
features & changes that improves the ENTIRE Minecraft experience. However still, the goal of this modpack is to stay as close as possible to "vanilla OptiFine." Hence,
there's no need to worry about mods that add content or change core game mechanics (as those are not included). We're just cloning the OptiFine experience, but
making it better!

* The mods in this modpack are categorized into [Performance](#performance), [OptiFine Features](#optifine-features), [Utility](#utility), [Extra Features](#extra-features),
  and [Libraries](#libraries).
* There are [Optional Mods](#optional) included in each release, and you can pick and choose which one you'd like to use.

#### Quick Note

This modpack is actually the personal modpack I use, and I thought it'd be a good idea to share it properly on GitHub so everybody else can use it! (It also makes it easier
for me to force it down my friends' throats 😅). Hope you guys enjoy it.

## How to Install & Use

`This is for the Vanilla Minecraft Launcher`

1. [Download Fabric](https://fabricmc.net/use/installer/) & install the Minecraft version you'd like to use.
2. [Download NANO](https://github.com/SirDanielIII/NANO/releases/). **Make sure the version you install corresponds with the correct Minecraft version!**
3. Unzip the file. (If you don't know how to do this... please Google it).
4. Locate the folder that Minecraft resides in, and go into the `mods` folder.
    * If there's no `mods` folder, just create it in the Minecraft directory.
    * If you need help locating the Minecraft folder, see [Windows](#windows) & [macOS](#macos).
5. **DELETE ANY PREVIOUS MODS CURRENTLY IN THE `mods` FOLDER, OR MOVE THEM INTO A FOLDER INSIDE SO THEY'RE OUT OF THE WAY.**
6. Copy & paste the JARs from the NANO folder into mods
    * Make sure the JARs are sitting in `mods` and not a folder inside `mods`!
    * Don't forget to copy-paste any JARs from NANO's "Optional" folder as well!
    * Ignore the following folders if they're present: `autotip` `memory_repo`
7. Open the Minecraft Launcher
8. Select the Fabric profile you want to run (E.G. fabric-loader-1.19.4) and press play!
    * [Optional] You can give your Minecraft profile more RAM. To do this, find the profile you want to edit in the "Installations" tab. Then click on the three dots to the right,
      then edit. Finally, change the number in `Xmx2G` to something like `Xmx6G` if you'd like to give Minecraft 6GB of RAM.
9. Launch the game & enjoy the frames. 🙂

### How To Find `mods` Folder:

#### Windows

1. Press `Windows + R` or open File Explorer.
2. Enter `%appdata%`.
3. Open the `.minecraft` folder.

#### macOS

1. On your desktop, click on `Go` and press `Computer`.
2. Click into your storage drive.
3. Navigate: `Users → [Your Username] → Library → Application Support → minecraft`

## Mod List

Note: Many of the descriptions are stolen and/or AI generated from the mods' original posts.

`✅ → Included` `🟡 → Awaiting Update` `❌ → Not Included`

### Performance

These mods aim towards making your FPS go brrrr.

| Name                                                                                | Author                                                       | 1.16.5 | 1.17.1 | 1.18.2 | 1.19.4 | 1.20.6 | 1.21 | Description                                                                                                                                                                                                                   |
|-------------------------------------------------------------------------------------|--------------------------------------------------------------|--------|--------|--------|--------|--------|------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Concurrent Chunk Management Engine (Fabric)](https://modrinth.com/mod/c2me-fabric) | [ishland](https://modrinth.com/user/ishland)                 | ❌      | ❌      | ✅      | ✅      | ✅      | ✅    | Designed to improve chunk performance. <br/><br/>⚠️ Crashes on 1.17.1.                                                                                                                                                        |
| [Enhanced Block Entities](https://modrinth.com/mod/ebe)                             | [FoundationGames](https://modrinth.com/user/FoundationGames) | ✅      | ✅      | ✅      | ✅      | 🟡     | ✅    | Increases block entity rendering performance.                                                                                                                                                                                 |
| [Entity Culling](https://modrinth.com/mod/entityculling)                            | [tr7zw](https://modrinth.com/user/tr7zw)                     | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Skips rendering non-visible Blocks/Entities.                                                                                                                                                                                  |
| [Hydrogen](https://modrinth.com/mod/hydrogen)                                       | [jellysquid3](https://modrinth.com/user/jellysquid3)         | ✅      | ✅      | ❌      | ❌      | ❌      | ❌    | Reduces Minecraft's memory usage.                                                                                                                                                                                             |
| [FerriteCore](https://modrinth.com/mod/ferrite-core)                                | [malte0811](https://modrinth.com/user/malte0811)             | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Reduces Minecraft's memory usage.                                                                                                                                                                                             |
| [ImmediatelyFast](https://modrinth.com/mod/immediatelyfast)                         | [RaphiMC](https://modrinth.com/user/RaphiMC)                 | ❌      | ❌      | ✅      | ✅      | ✅      | ✅    | Improves immediate mode rendering performance.                                                                                                                                                                                |
| [Indium](https://modrinth.com/mod/indium)                                           | [comp500](https://modrinth.com/user/comp500)                 | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Sodium addon for rendering optimization.                                                                                                                                                                                      |
| [Krypton](https://modrinth.com/mod/krypton)                                         | [astei](https://modrinth.com/user/astei)                     | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Optimizes Minecraft networking stack.                                                                                                                                                                                         |
| [LazyDFU](https://modrinth.com/mod/lazydfu)                                         | [astei](https://modrinth.com/user/astei)                     | ✅      | ✅      | ✅      | ✅      | ✅      | 🟡   | Defers unnecessary initialization work.                                                                                                                                                                                       |
| [Lithium](https://modrinth.com/mod/lithium)                                         | [jellysquid3](https://modrinth.com/user/jellysquid3)         | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Optimizes systems without changing vanilla mechanics.                                                                                                                                                                         |
| [Memory Leak Fix](https://modrinth.com/mod/memoryleakfix)                           | [fxmorin](https://modrinth.com/user/fxmorin)                 | ✅      | ❌      | ❌      | ✅      | ✅      | 🟡   | Fixes multiple memory leaks in Minecraft. <br/><br/>⚠️ Crashes on 1.17.1-1.18.2.                                                                                                                                              |
| [ModernFix](https://modrinth.com/mod/modernfix)                                     | [embeddedt](https://modrinth.com/user/embeddedt)             | ✅      | ❌      | ✅      | ✅      | ✅      | ✅    | Improves performance, reduces memory usage, and fixes bugs.                                                                                                                                                                   |
| [More Culling](https://modrinth.com/mod/moreculling)                                | [fxmorin](https://modrinth.com/user/fxmorin)                 | ❌      | ❌      | ✅      | ✅      | ✅      | 🟡   | Improves culling for performance.                                                                                                                                                                                             |
| [Noisium](https://modrinth.com/mod/noisium)                                         | [Steveplays](https://modrinth.com/user/Steveplays)           | ❌      | ❌      | ❌      | ❌      | ✅      | ✅    | Optimises world-gen for a better performance.                                                                                                                                                                                 |
| [Nvidium](https://modrinth.com/mod/nvidium)                                         | [cortex](https://modrinth.com/user/cortex)                   | ❌      | ❌      | ❌      | ✅      | ✅      | ✅    | Boosts FPS by using Nvidia black f**king magic.  <br/><br/>⚠️ The mod only works on Nvidia 16 series+ systems; will disable itself if the requirements aren't met and/or if shaders are enabled. Mod may also crash the game. |
| [Noxesium](https://modrinth.com/mod/noxesium)                                       | [Aeltumn](https://modrinth.com/user/Aeltumn)                 | ❌      | ❌      | ❌      | ✅      | ✅      | 🟡   | Speeds up custom model rendering and UIs.                                                                                                                                                                                     |
| [Sodium](https://modrinth.com/mod/sodium)                                           | [jellysquid3](https://modrinth.com/user/jellysquid3)         | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Implements modern rendering engine for better performance.                                                                                                                                                                    |
| [Phosphor](https://modrinth.com/mod/phosphor)                                       | [jellysquid3](https://modrinth.com/user/jellysquid3)         | ✅      | ❌      | ❌      | ❌      | ❌      | ❌    | Rewrites light engine for performance and fixes.   <br/><br/>✏️ Replaces [Starlight](https://modrinth.com/mod/starlight) for 1.16.5.                                                                                          |
| [Starlight](https://modrinth.com/mod/starlight)                                     | [spottedleaf](https://modrinth.com/user/spottedleaf)         | ❌      | ✅      | ✅      | ✅      | ❌      | ❌    | Rewrites light engine for performance and fixes. <br/><br/>✏️ [Discontinued after 1.20.4](https://gist.github.com/Spottedleaf/6cc1acdd03a9b7ac34699bf5e8f1b85c)                                                               |
| [Smooth Boot (Fabric)](https://modrinth.com/mod/smoothboot-fabric)                  | [UltimateBoomer](https://modrinth.com/user/UltimateBoomer)   | ✅      | ✅      | ✅      | ✅      | ❌      | ❌    | Improves and tweaks Minecraft CPU scheduling. <br/><br/>✏️ Replaces [ThreadTweak](https://modrinth.com/mod/threadtweak) for 1.16.5-1.19.4.                                                                                    |
| [ThreadTweak](https://modrinth.com/mod/threadtweak)                                 | [getchoo](https://modrinth.com/user/getchoo)                 | ❌      | ❌      | ❌      | ❌      | ✅      | 🟡   | Improves and tweaks Minecraft CPU scheduling. <br/><br/>✏️ Replaces [Smooth Boot (Fabric)](https://modrinth.com/mod/smoothboot-fabric) for 1.20+.                                                                             |

### OptiFine Features

These mods should emulate all if not most of OptiFine's features.

| Name                                                                            | Author                                                      | 1.16.5 | 1.17.1 | 1.18.2 | 1.19.4 | 1.20.6 | 1.21 | Description                                                                                                                                                                                                                               |
|---------------------------------------------------------------------------------|-------------------------------------------------------------|--------|--------|--------|--------|--------|------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Animatica](https://modrinth.com/mod/animatica)                                 | [FundationGames](https://modrinth.com/user/FoundationGames) | ❌      | ✅      | ✅      | ✅      | ✅      | ✅    | Adds support for loading MCPatcher/OptiFine animated texture format.                                                                                                                                                                      |
| [Capes](https://modrinth.com/mod/capes)                                         | [caelthecolher](https://modrinth.com/user/caelthecolher)    | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Allows the use of capes from Optifine, LabyMod, and MinecraftCapes Mod. <br/><br/>✏️ 1.16.5 version from [CurseForge](https://www.curseforge.com/minecraft/mc-mods/capes/files/all?page=1&pageSize=20&version=1.16.5&gameVersionTypeId=4) |
| [CIT Resewn](https://modrinth.com/mod/cit-resewn)                               | [shsupercm](https://modrinth.com/user/shsupercm)            | ❌      | ✅      | ✅      | ✅      | 🟡     | 🟡   | Enables resourcepacks to replace item appearances based on conditions.                                                                                                                                                                    |
| [Continuity](https://modrinth.com/mod/continuity)                               | [peppercode1](https://modrinth.com/user/peppercode1)        | ❌      | ✅      | ✅      | ✅      | ✅      | ✅    | Enables connected textures & Optifine-format emissive textures.                                                                                                                                                                           |
| [(EMF) Entity Model Features](https://modrinth.com/mod/entity-model-features)   | [Traben](https://modrinth.com/user/Traben)                  | ❌      | ❌      | ✅      | ✅      | ✅      | ✅    | Adds support for OptiFine's Custom Entity Models (CEM).                                                                                                                                                                                   |
| [(ETF) Entity Texture Features](https://modrinth.com/mod/entitytexturefeatures) | [Traben](https://modrinth.com/user/Traben)                  | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Adds emissive, random & custom texture support for entities.                                                                                                                                                                              |
| [Fabrishot](https://modrinth.com/mod/fabrishot)                                 | [ramidzkh](https://modrinth.com/user/ramidzkh)              | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Enables taking screenshots larger than the game resolution (e.g., 8K).                                                                                                                                                                    |
| [FabricSkyBoxes](https://modrinth.com/mod/fabricskyboxes)                       | [AMereBagatelle](https://modrinth.com/user/AMereBagatelle)  | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Allows defining custom skyboxes in resource packs.                                                                                                                                                                                        |
| [FabricSkyBoxes Interop](https://modrinth.com/mod/fabricskyboxes-interop)       | [FlashyReese](https://modrinth.com/user/FlashyReese)        | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Provides FabricSkyBoxes Interoperability for MCPatcher/OptiFine Skies.                                                                                                                                                                    |
| [Iris Shaders](https://modrinth.com/mod/iris)                                   | [coderbot](https://modrinth.com/user/coderbot)              | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Introduces shader support.                                                                                                                                                                                                                |
| [LambDynamicLights](https://modrinth.com/mod/lambdynamiclights)                 | [LambdAurora](https://modrinth.com/user/LambdAurora)        | ✅      | ✅      | ✅      | ✅      | 🟡     | 🟡   | Adds dynamic lights for torches, etc.                                                                                                                                                                                                     |
| [Ok Zoomer](https://modrinth.com/mod/ok-zoomer)                                 | [Ennui](https://modrinth.com/user/Ennui)                    | ✅      | ✅      | ❌      | ❌      | ❌      | ❌    | Adds a highly-configurable zoom key. <br/><br/>✏️ Not included in 1.18.2+ as it's basically cheating.                                                                                                                                     |
| [Colormatic](https://modrinth.com/mod/colormatic)                               | [kvverti](https://modrinth.com/user/kvverti)                | ❌      | ✅      | ✅      | ❓      | ❌      | ❌    | Offers compatibility with OptiFine's custom colours (color.properties).                                                                                                                                                                   |
| [Polytone](https://modrinth.com/mod/polytone)                                   | [MehVahdJukaar](https://modrinth.com/user/MehVahdJukaar)    | ❌      | ❌      | ❌      | ❌      | ✅      | ✅    | Offers backwards compatibility for OptiFine's custom colours (color.properties).                                                                                                                                                          |
| [Logical Zoom](https://modrinth.com/mod/logical-zoom)                           | [LogicalGeekBoy](https://modrinth.com/user/LogicalGeekBoy)  | ❌      | ❌      | ✅      | ✅      | ✅      | ✅    | Adds a zoom button similar to OptiFine's.                                                                                                                                                                                                 |
| [OptiGUI](https://modrinth.com/mod/optigui)                                     | [opekope2](https://modrinth.com/user/opekope2)              | ❌      | ❌      | ✅      | ✅      | ✅      | ✅    | Enables texture customization of in-game GUIs with resource packs.                                                                                                                                                                        |
| [Sodium Extra](https://modrinth.com/mod/sodium-extra)                           | [FlashyReese](https://modrinth.com/user/FlashyReese)        | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Brings OptiFine's eye-candy options to Sodium, with performance improvements.                                                                                                                                                             |

### Utility

These are included to improve the existing features in Minecraft.

| Name                                                                      | Author                                                        | 1.16.5 | 1.17.1 | 1.18.2 | 1.19.4 | 1.20.6 | 1.21 | Description                                                                                                                                                                        |
|---------------------------------------------------------------------------|---------------------------------------------------------------|--------|--------|--------|--------|--------|------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [AdvancementInfo](https://modrinth.com/mod/advancementinfo)               | [Giselbaer](https://modrinth.com/user/Giselbaer)              | ✅      | ✅      | ✅      | ✅      | ✅      | 🟡   | Enlarges the default advancements UI and adds an info panel.                                                                                                                       |
| [Audio Output](https://www.curseforge.com/minecraft/mc-mods/audio-output) | [maximumgame](https://www.curseforge.com/members/maximumgame) | ✅      | ✅      | ❌      | ❌      | ❌      | ❌    | Easily change Minecraft's audio output device without restarting the game.                                                                                                         |
| [Better Statistics Screen](https://modrinth.com/mod/better-stats)         | [TheCSDev](https://modrinth.com/user/TheCSDev)                | ❌      | ❌      | ✅      | ✅      | ✅      | ✅    | Improves the usefulness of the default statistics screen.                                                                                                                          |
| [Centered Crosshair](https://modrinth.com/mod/centered-crosshair)         | [JustAlittleWolf](https://modrinth.com/user/JustAlittleWolf)  | ❌      | ❌      | ❌      | ❌      | ✅      | ✅    | Corrects the crosshair misalignment bug ([MC-157252](https://bugs.mojang.com/browse/MC-157252)).                                                                                   |
| [Dynamic FPS](https://modrinth.com/mod/dynamic-fps)                       | [juliand665](https://modrinth.com/user/juliand665)            | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Automatically adjusts rendering speed based on focus or visibility.                                                                                                                |
| [Language Reload](https://modrinth.com/mod/language-reload)               | [Jerozgen](https://modrinth.com/user/Jerozgen)                | ❌      | ✅      | ✅      | ✅      | ✅      | ✅    | Introduces quality of life changes related to languages.                                                                                                                           |
| [MixinTrace](https://modrinth.com/mod/mixintrace)                         | [comp500](https://modrinth.com/user/comp500)                  | ❌      | ✅      | ✅      | ✅      | ✅      | 🟡   | Adds mixin details to crash reports for debugging.                                                                                                                                 |
| [Mod Menu](https://modrinth.com/mod/modmenu)                              | [Prospector](https://modrinth.com/user/Prospector)            | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Provides a mod menu to view installed mods.                                                                                                                                        |
| [No Telemetry](https://modrinth.com/mod/no-telemetry)                     | [kb1000](https://modrinth.com/user/kb1000)                    | ❌      | ❌      | ✅      | ✅      | ✅      | ✅    | Disables telemetry introduced in Minecraft 21w38a.                                                                                                                                 |
| [Not Enough Crashes](https://modrinth.com/mod/notenoughcrashes)           | [natanfudge](https://modrinth.com/user/natanfudge)            | ❌      | ❌      | ❌      | ✅      | ✅      | 🟡   | Allows resuming gameplay after Minecraft crashes.  <br/><br/>⚠️ Crashes in 1.18.2 and before.                                                                                      |
| [Reese's Sodium Options](https://modrinth.com/mod/reeses-sodium-options)  | [FlashyReese](https://modrinth.com/user/FlashyReese)          | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Enhances Sodium's Options Screen for better user experience.                                                                                                                       |
| [Remove Reloading Screen](https://modrinth.com/mod/rrls)                  | [dima_dencep](https://modrinth.com/user/dima_dencep)          | ✅      | ❌      | ✅      | ✅      | ✅      | ✅   | Loads resource packs in the background & removes its loading screen.<br/><br/>⚠️ Warning: Replay Mod exports will have a high chance of failing if this is installed alongside it. |
| [fast-ip-ping](https://modrinth.com/mod/fast-ip-ping)                     | [fallen-breath](https://modrinth.com/user/fallen-breath)      | ✅      | ✅      | ❌      | ❌      | ❌      | ❌    | Fixes "Can't connect to server" on refresh.                                                                                                                                        |
| [Server Pinger Fixer](https://modrinth.com/mod/serverpingerfixer)         | [JustAlittleWolf](https://modrinth.com/user/JustAlittleWolf)  | ❌      | ❌      | ✅      | ✅      | ✅      | ✅    | Improves how servers in the multiplayer list are pinged.                                                                                                                           |
| [ToolTipFix](https://modrinth.com/mod/tooltipfix)                         | [kyrptonaught](https://modrinth.com/user/kyrptonaught)        | ❌      | ✅      | ✅      | ✅      | ✅      | 🟡   | Corrects tooltips to prevent them from running off the screen.                                                                                                                     |
| [Your Options Shall Be Respected (YOSBR)](https://modrinth.com/mod/yosbr) | [shedaniel](https://modrinth.com/user/shedaniel)              | ✅      | ✅      | ✅      | ✅      | ✅      | 🟡   | Preserves settings across different Minecraft versions.                                                                                                                            |

### Extra Features

Doesn't add new content and/or change the core game mechanics. They just complement the current experience.

| Name                                                                        | Author                                                         | 1.16.5 | 1.17.1 | 1.18.2 | 1.19.4 | 1.20.6 | 1.21 | Description                                                                                |
|-----------------------------------------------------------------------------|----------------------------------------------------------------|--------|--------|--------|--------|--------|------|--------------------------------------------------------------------------------------------|
| [Controlling](https://modrinth.com/mod/controlling)                         | [jaredlll08](https://modrinth.com/user/jaredlll08)             | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Adds a search bar to the Key-Bindings menu.                                                |
| [Disable Custom Worlds Advice](https://modrinth.com/mod/dcwa)               | [rdvdev2](https://modrinth.com/user/rdvdev2)                   | ✅      | ✅      | ✅      | ✅      | 🟡     | 🟡   | Disables the "Experimental Features" warning for custom dimensions or settings.            |
| [Falling Leaves](https://modrinth.com/mod/fallingleaves)                    | [randommcsomethin](https://modrinth.com/user/randommcsomethin) | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Introduces a particle effect to leaf blocks.                                               |
| [More Chat History](https://modrinth.com/mod/morechathistory)               | [JackFred2](https://modrinth.com/user/JackFred2)               | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Increases the maximum length of chat history.                                              |
| [No Chat Reports](https://modrinth.com/mod/no-chat-reports)                 | [Aizistral](https://modrinth.com/user/Aizistral)               | ❌      | ❌      | ❌      | ✅      | ✅      | ✅    | Removes cryptographic signatures from chat messages in Minecraft 1.19.1+ (when possible).  |
| [Screenshot to Clipboard](https://modrinth.com/mod/screenshot-to-clipboard) | [comp500](https://modrinth.com/user/comp500)                   | ✅      | ✅      | ✅      | ✅      | ✅      | 🟡   | Copies screenshots to the clipboard.                                                       |
| [ViaFabricPlus](https://modrinth.com/mod/viafabricplus)                     | [FlorianMichael](https://modrinth.com/user/FlorianMichael)     | ❌      | ❌      | ❌      | ❌      | ✅      | ✅    | Allows seamless switching between Minecraft versions in Multiplayer.                       |
| [Technopig](https://modrinth.com/mod/technomodel)                           | [thecolonel63](https://modrinth.com/user/thecolonel63)         | ❌      | ❌      | ✅      | ✅      | ✅      | 🟡   | Adds a crown to any pig named "Technoblade". <br/><br/>⚠️ Doesn't boot properly on 1.17.1. |

### Libraries

These are needed for some mods to work properly.

| Name                                                                      | Author                                             | 1.16.5 | 1.17.1 | 1.18.2 | 1.19.4 | 1.20.6 | 1.21 | Description                                |
|---------------------------------------------------------------------------|----------------------------------------------------|--------|--------|--------|--------|--------|------|--------------------------------------------|
| [Cloth Config API](https://modrinth.com/mod/cloth-config)                 | [shedaniel](https://modrinth.com/user/shedaniel)   | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Required for Falling Leaves & More Culling |
| [Fabric API](https://modrinth.com/mod/fabric-api)                         | [modmuss50](https://modrinth.com/user/modmuss50)   | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Required for most mods                     |
| [Fabric Language Kotlin](https://modrinth.com/mod/fabric-language-kotlin) | [modmuss50](https://modrinth.com/user/modmuss50)   | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Required for Capes & OptiGUI               |
| [Searchables](https://modrinth.com/mod/searchables)                       | [jaredlll08](https://modrinth.com/user/jaredlll08) | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Required for Controlling                   |
| [TCDCommons API](https://modrinth.com/mod/Eldc1g37)                       | [TheCSDev](https://modrinth.com/user/TheCSDev)     | ❌      | ❌      | ❌      | ❌      | ❌      | ✅    | Required for Better Statistics Screen      |

### Optional

Fun mods that can be useful, and don't really belong in the core NANO package.

| Name                                                                          | Author                                               | 1.16.5 | 1.17.1 | 1.18.2 | 1.19.4 | 1.20.6 | 1.21 | Description                                                                                                                                                                                                                                                 |
|-------------------------------------------------------------------------------|------------------------------------------------------|--------|--------|--------|--------|--------|------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [AppleSkin](https://modrinth.com/mod/appleskin)                               | [squeek502](https://modrinth.com/user/squeek502)     | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Enhances food/hunger HUD with saturation display.                                                                                                                                                                                                           |
| [CraftPresence](https://modrinth.com/mod/craftpresence)                       | [CDAGaming_](https://modrinth.com/user/CDAGaming)    | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Customizes how you appear on Discord's Rich Presence while playing Minecraft.                                                                                                                                                                               |
| [Dark Loading Screen](https://modrinth.com/mod/dark-loading-screen)           | [A5b84](https://modrinth.com/user/A5b84)             | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Darkens the loading screen for a sleeker look.                                                                                                                                                                                                              |
| [LambdaControls](https://modrinth.com/mod/lambdacontrols)                     | [LambdAurora](https://modrinth.com/user/LambdAurora) | ✅      | ✅      | ❌      | ❌      | ❌      | ❌    | Enables controller support.                                                                                                                                                                                                                                 |
| [MidnightControls](https://modrinth.com/mod/midnightcontrols)                 | [Motschen](https://modrinth.com/user/Motschen)       | ❌      | ❌      | ✅      | ✅      | ✅      | ✅    | Enables controller support.                                                                                                                                                                                                                                 |
| [Plasmo Voice](https://modrinth.com/plugin/plasmo-voice)                      | [kpids](https://modrinth.com/user/kpids)             | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Proximity voice chat with advanced features.                                                                                                                                                                                                                |
| [Presence Footsteps](https://modrinth.com/mod/presence-footsteps)             | [Sollace](https://modrinth.com/user/Sollace)         | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | Adds dynamic block sound effects to player movement.                                                                                                                                                                                                        |
| [Replay Mod](https://modrinth.com/mod/replaymod)                              | [Johni0702](https://modrinth.com/user/Johni0702)     | ✅      | ✅      | ✅      | ✅      | 🟡     | 🟡   | Record, replay, and share your Minecraft adventures. <br/><br/>⚠️ Regarding 1.20.2+, in my testing, replay files can't be played back if you join a proxy server, and then record after switching servers in the same session (at least with this modpack). |                                                                                                                    |
| [Sound Physics](https://modrinth.com/mod/soundphysics)                        | [thedocruby](https://modrinth.com/user/thedocruby)   | ❌      | ✅      | ✅      | ❌      | ❌      | ❌    | Adds realistic sound attenuation, reverberation, and absorption through blocks. <br/><br/>✏️ Replaces [Sound Physics Remastered](https://modrinth.com/mod/sound-physics-remastered) for 1.17.1 & 1.18.2                                                     |
| [Sound Physics Remastered](https://modrinth.com/mod/sound-physics-remastered) | [henkelmax](https://modrinth.com/user/henkelmax)     | ❌      | ❌      | ❌      | ✅      | ✅      | ✅    | Adds realistic sound attenuation, reverberation, and absorption through blocks. <br/><br/>✏️ Replaces [Sound Physics](https://modrinth.com/mod/soundphysics) for 1.19.4+                                                                                    |
| [World Edit](https://modrinth.com/plugin/worldedit)                           | [me4502](https://modrinth.com/user/me4502)           | ✅      | ✅      | ✅      | ✅      | ✅      | ✅    | In-game map editor for Minecraft. <br/><br/>✏️ 1.16.5 to 1.19.4 versions are downloaded from [CurseForge](https://www.curseforge.com/minecraft/mc-mods/worldedit)                                                                                           |
| [pv-addon-replaymod](https://modrinth.com/mod/pv-addon-replaymod)             | [kpids](https://modrinth.com/user/kpids)             | ❌      | ❌      | ❌      | ✅      | 🟡     | 🟡   | Records voice chat in ReplayMod recordings. <br/><br/>✏️ Requires [Plasmo Voice](https://modrinth.com/plugin/plasmo-voice) & Replay Mod.                                                                                                                    |                                                                                 |
| [pv-addon-sound-physics](https://modrinth.com/mod/pv-addon-soundphysics/)     | [kpids](https://modrinth.com/user/kpids)             | ❌      | ❌      | ❌      | ✅      | ✅      | 🟡   | Integrates sound physics with [Plasmo Voice](https://modrinth.com/plugin/plasmo-voice). <br/><br/>✏️ Requires [Plasmo Voice](https://modrinth.com/plugin/plasmo-voice) & Sound Physics Remastered.                                                          |
| [pv-addon-sculk](https://modrinth.com/plugin/pv-addon-sculk)                  | [kpids](https://modrinth.com/user/kpids)             | ❌      | ❌      | ❌      | ✅      | ✅      | 🟡   | Warden and sculk sensors are triggered with proximity voice chat. <br/><br/>✏️ Requires [Plasmo Voice](https://modrinth.com/plugin/plasmo-voice).                                                                                                           |
