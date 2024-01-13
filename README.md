# Na, No OptiFine (NANO)

The definitive Fabric performance modpack that aims to eliminate the need for OptiFine, **FOREVER**.

Note: 1.16.5 to 1.17.2 packs will release eventually... life is too busy :(

<details>

## What is [OptiFine](https://www.optifine.net/home) & [Sodium](https://modrinth.com/mod/sodium)?

OptiFine is a very popular optimization mod that helps improve Minecraft's performance, and adds extra features that the vanilla client doesn't have. However, even while being a
performance mod, it's still very sluggish.

* E.G. Booting up the game or even changing resource packs takes foreverrrrrr...

Furthermore, the closed-source nature and intrusive characteristics of OptiFine pose challenges for other developers aiming to produce mods that are compatible with it.

Sodium is the free & open-source alternative to OptiFine that actually has **better performance**, and is compatible with a wide range of the Fabric mod ecosystem.
However, by itself, it lacks many of the beloved features from OptiFine, such as a zoom key, shader support, dynamic lighting, extreme customization with resource packs, etc.,
which can make transitioning out of OptiFine very difficult.
</details>

## So What Does This Modpack Do?

#### `Modpack Revision: 2`

Changes from Revision 1:
<details>

* Added [fast-ip-ping](https://modrinth.com/mod/fast-ip-ping)
* Added [Noxesium](https://modrinth.com/mod/noxesium)
* Moved [Remove Reloading Screen](https://modrinth.com/mod/rrls) to Optional Mods as it bugs out Replay Mod when exporting
* Removed [Better Beds](https://modrinth.com/mod/better-beds) because it does not render beds properly (plus it doesn't do much)

</details>

By using [the following mods](#mod-list), we're able to incorporate ALL of OptiFine's features, while still using Sodium! In addition, there are some quality of life
features & changes that enhance the Minecraft experience. However, the aim of this modpack is to stay as close to the "vanilla OptiFine" Minecraft experience as possible. This
means that there are no mods that add content or change core game mechanics. It's just cloning the OptiFine experience, but making it better!

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
5. DELETE ANY PREVIOUS MODS CURRENTLY IN THE `mods` FOLDER, OR MOVE THEM INTO A FOLDER INSIDE SO THEY'RE OUT OF THE WAY.
6. Copy & paste the JARs from the NANO folder into mods
    * Make sure the JARs are sitting in `mods` and not a folder inside `mods`!
    * Don't forget to copy-paste any JARs from NANO's "Optional" folder as well!
    * Ignore the following folders if they're present: `autotip` `memory_repo`
7. Open the Minecraft Launcher
8. Select the Fabric profile you want to run (E.G. fabric-loader-1.19.4) and press play!
    * [Optional] You can give your Minecraft profile more RAM. To do this, find the profile you want to edit in the "Installations" tab. Then click on the three dots to the right,
      then edit. Finally, change the number in `Xmx2G` to something like `Xmx6G` if you'd like to give Minecraft 6GB of RAM.
9. If Minecraft launches, and you get this message, just continue and ignore it:
   ![img.png](images/iris_complains_about_notenoughcrashes.png)

<details>

### Windows

1. Press `Windows + R`, type `%appdata%` and press enter.
2. Go into the `.minecraft` folder.

### macOS

1. On your desktop, click on `Go` and press `Computer`.
2. Click into your storage drive.
3. Navigate: `Users → [Your Username] → Library → Application Support → minecraft`

</details>

## Mod List

Note: Many of the descriptions are copied from the mods' original posts.

`✅ → Included` `🟡 → Not Included (awaiting update)` `❌ → Not Included`

### Performance <sup>[14]</sup>

These mods aim towards making your FPS go brrrr.

| Name                                                        | Author                                                       | 1.16.5 | 1.17.1 | 1.18.2 | 1.19.4 | 1.20.1 | 1.20.2 | 1.20.4 | Description                                                                                                                    |
|-------------------------------------------------------------|--------------------------------------------------------------|--------|--------|--------|--------|--------|--------|--------|--------------------------------------------------------------------------------------------------------------------------------|
| [Enhanced Block Entities](https://modrinth.com/mod/ebe)     | [FoundationGames](https://modrinth.com/user/FoundationGames) | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Increases the performance of block entity rendering.                                                                           |
| [Entity Culling](https://modrinth.com/mod/entityculling)    | [tr7zw](https://modrinth.com/user/tr7zw)                     | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Uses async path-tracing to skip rendering Block/Entities that are not visible.                                                 |
| [FerriteCore](https://modrinth.com/mod/ferrite-core)        | [malte0811](https://modrinth.com/user/malte0811)             | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Reduces Minecraft's memory usage.                                                                                              |
| [ImmediatelyFast](https://modrinth.com/mod/immediatelyfast) | [RaphiMC](https://modrinth.com/user/RaphiMC)                 | ❌      | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | Improves the immediate mode rendering performance of the Minecraft client.                                                     |
| [Indium](https://modrinth.com/mod/indium)                   | [comp500](https://modrinth.com/user/comp500)                 | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | An addon for the rendering optimization mod, Sodium.                                                                           |
| [Krypton](https://modrinth.com/mod/krypton)                 | [astei](https://modrinth.com/user/astei)                     | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Attempts to optimize the Minecraft networking stack.                                                                           |
| [LazyDFU](https://modrinth.com/mod/lazydfu)                 | [astei](https://modrinth.com/user/astei)                     | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Defers unnecessary initialization work so that it is only performed if required.                                               |
| [Lithium](https://modrinth.com/mod/lithium)                 | [jellysquid3](https://modrinth.com/user/jellysquid3)         | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | An optimization mod that improves a number of systems without changing vanilla mechanics.                                      |
| [Memory Leak Fix](https://modrinth.com/mod/memoryleakfix)   | [fxmorin](https://modrinth.com/user/fxmorin)                 | ✅      | ✅      | ❌      | ✅      | ✅      | ✅      | ✅      | A modern, general-purpose optimization mod for Minecraft.                                                                      |
| [ModernFix](https://modrinth.com/mod/modernfix)             | [embeddedt](https://modrinth.com/user/embeddedt)             | ✅      | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | Improves performance, reduces memory usage, and fixes many bugs in modern Minecraft versions.                                  |
| [More Culling](https://modrinth.com/mod/moreculling)        | [fxmorin](https://modrinth.com/user/fxmorin)                 | ❌      | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | Changes how multiple types of culling are handled in order to improve performance.                                             |
| [Noxesium](https://modrinth.com/mod/noxesium)               | [Aeltumn](https://modrinth.com/user/Aeltumn)                 | ❌      | ❌      | ❌      | ✅      | ✅      | ✅      | ✅      | Speeds up custom model rendering, recolorable models beacon beam rendering, and massively speeds up rendering of on-screen UIs |
| [Sodium](https://modrinth.com/mod/sodium)                   | [jellysquid3](https://modrinth.com/user/jellysquid3)         | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Implements a modern rendering engine for Minecraft, which greatly improves performance.                                        |
| [Starlight](https://modrinth.com/mod/starlight)             | [spottedleaf](https://modrinth.com/user/spottedleaf)         | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Rewrites the light engine to fix lighting performance and lighting errors.                                                     |

### OptiFine Features <sup>[14]</sup>

These mods should emulate all if not most of OptiFine's features.

| Name                                                                            | Author                                                      | 1.16.5 | 1.17.1 | 1.18.2 | 1.19.4 | 1.20.1 | 1.20.2 | 1.20.4 | Description                                                                                                                                                                                |
|---------------------------------------------------------------------------------|-------------------------------------------------------------|--------|--------|--------|--------|--------|--------|--------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Animatica](https://modrinth.com/mod/animatica)                                 | [FundationGames](https://modrinth.com/user/FoundationGames) | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Adds ability to load the MCPatcher/OptiFine [animated texture format](https://github.com/sp614x/optifine/blob/master/OptiFineDoc/doc/custom_animations.txt).                               |
| [Capes](https://modrinth.com/mod/capes)                                         | [caelthecolher](https://modrinth.com/user/caelthecolher)    | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Lets you use capes from Optifine, LabyMod, and the MinecraftCapes Mod.                                                                                                                     |
| [CIT Resewn](https://modrinth.com/mod/cit-resewn)                               | [shsupercm](https://modrinth.com/user/shsupercm)            | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Allows resourcepacks to replace the appearance of items when they meet certain conditions.<br/><br/>✏️ The 1.20.4 version is ported from [here.](https://github.com/dicedpixels/CITResewn) |
| [Continuity](https://modrinth.com/mod/continuity)                               | [peppercode1](https://modrinth.com/user/peppercode1)        | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Allows for connected textures & Optifine-format emissive textures.                                                                                                                         |
| [(EMF) Entity Model Features](https://modrinth.com/mod/entity-model-features)   | [Traben](https://modrinth.com/user/Traben)                  | ❌      | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | Adds support for OptiFine's Custom Entity Models (CEM).                                                                                                                                    |
| [(ETF) Entity Texture Features](https://modrinth.com/mod/entitytexturefeatures) | [Traben](https://modrinth.com/user/Traben)                  | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Emissive, Random & Custom texture support for entities in resourcepacks (like Optifine but for Fabric).                                                                                    |
| [Fabrishot](https://modrinth.com/mod/fabrishot)                                 | [ramidzkh](https://modrinth.com/user/ramidzkh)              | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Let's you take super large screenshots (such as 4K or 8K).                                                                                                                                 |
| [FabricSkyBoxes](https://modrinth.com/mod/fabricskyboxes)                       | [AMereBagatelle](https://modrinth.com/user/AMereBagatelle)  | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Allows resource packs to define custom skyboxes.                                                                                                                                           |
| [FabricSkyBoxes Interop](https://modrinth.com/mod/fabricskyboxes-interop)       | [FlashyReese](https://modrinth.com/user/FlashyReese)        | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | FabricSkyBoxes Interoperability for MCPatcher/OptiFine Skies.                                                                                                                              |
| [Iris Shaders](https://modrinth.com/mod/iris)                                   | [coderbot](https://modrinth.com/user/coderbot)              | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | SHADER SUPPORT :D                                                                                                                                                                          |
| [LambDynamicLights](https://modrinth.com/mod/lambdynamiclights)                 | [LambdAurora](https://modrinth.com/user/LambdAurora)        | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | 🟡     | Dynamic lights for torches, etc.                                                                                                                                                           |
| [Logical Zoom](https://modrinth.com/mod/logical-zoom)                           | [LogicalGeekBoy](https://modrinth.com/user/LogicalGeekBoy)  | ❌      | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | Adds a zoom button similar to OptiFine's.                                                                                                                                                  |
| [OptiGUI](https://modrinth.com/mod/optigui)                                     | [opekope2](https://modrinth.com/user/opekope2)              | ❌      | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | Allows the texture customization of in-game GUIs with resource packs.                                                                                                                      |
| [Sodium Extra](https://modrinth.com/mod/sodium-extra)                           | [FlashyReese](https://modrinth.com/user/FlashyReese)        | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Aims to bring most of OptiFine's eye-candy options to Sodium, alongside visual bugfixes & other performance options.                                                                       |

### Utility <sup>[12]</sup>

These are included to improve the existing features in Minecraft.

| Name                                                                      | Author                                                   | 1.16.5 | 1.17.1 | 1.18.2 | 1.19.4 | 1.20.1 | 1.20.2 | 1.20.4 | Description                                                                                                                                          |
|---------------------------------------------------------------------------|----------------------------------------------------------|--------|--------|--------|--------|--------|--------|--------|------------------------------------------------------------------------------------------------------------------------------------------------------|
| [AdvancementInfo](https://modrinth.com/mod/advancementinfo)               | [Giselbaer](https://modrinth.com/user/Giselbaer)         | ✅      | ✅      | ✅      | ✅      | ✅      | ❌      | ✅      | Replaces the default advancements UI with an enlarged version that also has an info panel.                                                           |
| [Better Statistics Screen](https://modrinth.com/mod/better-stats)         | [TheCSDev](https://modrinth.com/user/TheCSDev)           | ❌      | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | Replaces the default statistics screen with one that's more useful.                                                                                  |
| [Dynamic FPS](https://modrinth.com/mod/dynamic-fps)                       | [juliand665](https://modrinth.com/user/juliand665)       | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Automatically reduces the speed at which Minecraft renders when it's not focused (to 1 FPS) or hidden (no renders at all).                           |
| [fast-ip-ping](https://modrinth.com/mod/fast-ip-ping)                     | [fallen-breath](https://modrinth.com/user/fallen-breath) | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Yeets the laggy reversed DNS lookup for pure IP server addresses (fixes "Can't connect to server" on refresh).                                       |
| [Language Reload](https://modrinth.com/mod/language-reload)               | [Jerozgen](https://modrinth.com/user/Jerozgen)           | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Adds quality of life changes related to languages.                                                                                                   |
| [MixinTrace](https://modrinth.com/mod/mixintrace)                         | [comp500](https://modrinth.com/user/comp500)             | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Adds a list of mixins (and Mixin configuration names) to classes in the stack trace to crash reports.                                                |
| [Mod Menu](https://modrinth.com/mod/modmenu)                              | [Prospector](https://modrinth.com/user/Prospector)       | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Adds a mod menu to view the list of mods you have installed.                                                                                         |
| [No Telemetry](https://modrinth.com/mod/no-telemetry)                     | [kb1000](https://modrinth.com/user/kb1000)               | ❌      | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | Disables the telemetry introduced in Minecraft 21w38a.                                                                                               |
| [Not Enough Crashes](https://modrinth.com/mod/notenoughcrashes)           | [natanfudge](https://modrinth.com/user/natanfudge)       | ✅      | ✅      | ❌      | ✅      | ❌      | ✅      | 🟡     | Allows you to go back to the title screen and keep playing if Minecraft crashes.   <br/><br/>✏️ Iris will crash in NANO-1.20.1-r1.0 for some reason. |
| [Reese's Sodium Options](https://modrinth.com/mod/reeses-sodium-options)  | [FlashyReese](https://modrinth.com/user/FlashyReese)     | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Replaces Sodium's Options Screen with intention of improving UX.                                                                                     |
| [ToolTipFix](https://modrinth.com/mod/tooltipfix)                         | [kyrptonaught](https://modrinth.com/user/kyrptonaught)   | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Fixes Tooltips from runnning off the screen.                                                                                                         |
| [Your Options Shall Be Respected (YOSBR)](https://modrinth.com/mod/yosbr) | [shedaniel](https://modrinth.com/user/shedaniel)         | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Keeps your settings when switching between different Minecraft versions.                                                                             |

### Extra Features <sup>[8]</sup>

Doesn't add new content and/or change the core game mechanics. They just complement the current experience.

| Name                                                                        | Author                                                         | 1.16.5 | 1.17.1 | 1.18.2 | 1.19.4 | 1.20.1 | 1.20.2 | 1.20.4 | Description                                                                                                                                                                             |
|-----------------------------------------------------------------------------|----------------------------------------------------------------|--------|--------|--------|--------|--------|--------|--------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Controlling](https://modrinth.com/mod/controlling)                         | [jaredlll08](https://modrinth.com/user/jaredlll08)             | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Adds a search bar to the Key-Bindings menu.                                                                                                                                             |
| [Falling Leaves](https://modrinth.com/mod/fallingleaves)                    | [randommcsomethin](https://modrinth.com/user/randommcsomethin) | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Adds a neat little particle effect to leaf blocks.                                                                                                                                      |
| [MidnightControls](https://modrinth.com/mod/midnightcontrols)               | [Motschen](https://modrinth.com/user/Motschen)                 | ❌      | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | Adds controller support.                                                                                                                                                                |
| [More Chat History](https://modrinth.com/mod/morechathistory)               | [JackFred2](https://modrinth.com/user/JackFred2)               | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Increases the maximum length of chat history.                                                                                                                                           |
| [No Chat Reports](https://modrinth.com/mod/no-chat-reports)                 | [Aizistral](https://modrinth.com/user/Aizistral)               | ❌      | ❌      | ❌      | ✅      | ✅      | ✅      | ✅      | Strips cryptographic signatures that since 1.19 are attached to every message sent in the chat (when possible).                                                                         |
| [Screenshot to Clipboard](https://modrinth.com/mod/screenshot-to-clipboard) | [comp500](https://modrinth.com/user/comp500)                   | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Screenshots are copied to the clipboard.                                                                                                                                                |
| [ViaFabricPlus](https://modrinth.com/mod/viafabricplus)                     | [FlorianMichael](https://modrinth.com/user/FlorianMichael)     | ❌      | ❌      | ❌      | ❌      | ✅      | ❌      | ✅      | Allows you to switch between different Minecraft versions on the fly (for Multiplayer / servers). <br/><br/>⚠️ Warning 1: Can be buggy sometimes. <br/>⚠️ Warning 2: Crashes on 1.20.2. |
| [Technopig](https://modrinth.com/mod/technomodel)                           | [thecolonel63](https://modrinth.com/user/thecolonel63)         | ❌      | ✅      | ✅      | ✅      | ✅      | ✅      | ✅      | Any pig with the name "Technoblade" will have a crown added to its head.                                                                                                                |

### Libraries <sup>[4]</sup>

These are needed for some mods to work properly.

| Name                                                                      | Author                                             | 1.16.5 | 1.17.1 | 1.18.2 | 1.19.4 | 1.20.1-1.20.2 | 1.20.4 | Description                                |
|---------------------------------------------------------------------------|----------------------------------------------------|--------|--------|--------|--------|---------------|--------|--------------------------------------------|
| [Cloth Config API](https://modrinth.com/mod/cloth-config)                 | [shedaniel](https://modrinth.com/user/shedaniel)   | ✅      | ✅      | ✅      | ✅      | ✅             | ✅      | Required for Falling Leaves & More Culling |
| [Fabric API](https://modrinth.com/mod/fabric-api)                         | [modmuss50](https://modrinth.com/user/modmuss50)   | ✅      | ✅      | ✅      | ✅      | ✅             | ✅      | Required for most mods                     |
| [Fabric Language Kotlin](https://modrinth.com/mod/fabric-language-kotlin) | [modmuss50](https://modrinth.com/user/modmuss50)   | ❌      | ❌      | ✅      | ✅      | ✅             | ✅      | Required for Capes, OptiGUI & OptiGlue     |
| [Searchables](https://modrinth.com/mod/searchables)                       | [jaredlll08](https://modrinth.com/user/jaredlll08) | ✅      | ✅      | ✅      | ✅      | ✅             | ✅      | Required for Controlling                   |

### Optional <sup>[11]</sup>

Fun mods that can be useful, and don't really belong in the core NANO package.

| Name                                                                          | Author                                               | 1.16.5 | 1.17.1 | 1.18.2 | 1.19.4 | 1.20.1-1.20.2 | 1.20.4 | Description                                                                                                                                                                                               |
|-------------------------------------------------------------------------------|------------------------------------------------------|--------|--------|--------|--------|---------------|--------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [AppleSkin](https://modrinth.com/mod/appleskin)                               | [squeek502](https://modrinth.com/user/squeek502)     | ✅      | ✅      | ✅      | ✅      | ✅             | ✅      | Adds food/hunger-related HUD improvements (E.G. Showing saturation, etc).                                                                                                                                 |
| [CraftPresence](https://modrinth.com/mod/craftpresence)                       | [CDAGaming_](https://modrinth.com/user/CDAGaming)    | ✅      | ✅      | ✅      | ✅      | ✅             | ✅      | Let's you completely customize the way others see you play Minecraft via Discord's Rich Presence API & the DiscordIPC API.                                                                                |
| [Dark Loading Screen](https://modrinth.com/mod/dark-loading-screen)           | [A5b84](https://modrinth.com/user/A5b84)             | ✅      | ✅      | ✅      | ✅      | ✅             | ✅      | Makes the loading screen darker.                                                                                                                                                                          |
| [Plasmo Voice](https://modrinth.com/plugin/plasmo-voice)                      | [kpids](https://modrinth.com/user/kpids)             | ✅      | ✅      | ✅      | ✅      | ✅             | ✅      | A proximity voice chat mod with audio positioning and lots of features.                                                                                                                                   |
| [Replay Mod](https://modrinth.com/mod/replaymod)                              | [Johni0702](https://modrinth.com/user/Johni0702)     | ✅      | ✅      | ✅      | ✅      | ✅             | ✅      | Allows you to record, replay and share your Minecraft experience.                                                                                                                                         |                                                                                                                    |
| [Remove Reloading Screen](https://modrinth.com/mod/rrls)                      | [dima_dencep](https://modrinth.com/user/dima_dencep) | ✅      | ❌      | ✅      | ✅      | ✅             | ✅      | Makes resource packs load in the background, allowing you to do other things while waiting.<br/><br/>⚠️ Warning: Replay Mod exports will have a high chance of failing if this is installed alongside it. |
| [Sound Physics Remastered](https://modrinth.com/mod/sound-physics-remastered) | [henkelmax](https://modrinth.com/user/henkelmax)     | ❌      | ❌      | ❌      | ✅      | ✅             | ✅      | Provides realistic sound attenuation, reverberation, and absorption through blocks.                                                                                                                       |
| [pv-addon-replaymod](https://modrinth.com/mod/pv-addon-replaymod)             | [kpids](https://modrinth.com/user/kpids)             | ❌      | ❌      | ❌      | ✅      | ✅             | ✅      | Allows you to record voice chat with ReplayMod. <br/><br/>✏️ Requires Plasmo Voice & Sound Physics Remastered.                                                                                            | *Requires Replay Mod & Plasmo Voice                                                                                |
| [pv-addon-sound-physics](https://modrinth.com/mod/pv-addon-soundphysics/)     | [kpids](https://modrinth.com/user/kpids)             | ❌      | ❌      | ❌      | ✅      | ✅             | ✅      | Makes sound physics affect Plasmo Voice. <br/><br/>✏️ Requires Plasmo Voice & Sound Physics Remastered.                                                                                                   |
| [Presence Footsteps](https://modrinth.com/mod/presence-footsteps)             | [Sollace](https://modrinth.com/user/Sollace)         | ✅      | ✅      | ✅      | ✅      | ✅             | ✅      | A sound mod that adds new and more dynamic sounds for every block the player walks on.                                                                                                                    |
| [World Edit](https://modrinth.com/plugin/worldedit)                           | [me4502](https://modrinth.com/user/me4502)           | ✅      | ✅      | ✅      | ✅      | ✅             | ✅      | Powerful in-game map editor tool for Minecraft. <br/><br/>✏️ 1.16.5 to 1.19.4 versions are downloaded from [CurseForge](https://www.curseforge.com/minecraft/mc-mods/worldedit)                           |
