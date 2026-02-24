<![CDATA[<div align="center">

# ⚔️ RPG Maker MV — Project I

**A Fantasy RPG built with RPG Maker MV**

[![Made with RPG Maker MV](https://img.shields.io/badge/Made%20with-RPG%20Maker%20MV-blue?style=for-the-badge&logo=data:image/png;base64,iVBORw0KGgo=)](https://www.rpgmakerweb.com/products/rpg-maker-mv)
[![JavaScript](https://img.shields.io/badge/Engine-JavaScript%20%2F%20HTML5-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Pixi.js](https://img.shields.io/badge/Renderer-Pixi.js-e91e63?style=for-the-badge)](https://pixijs.com/)
[![License](https://img.shields.io/badge/License-Proprietary-red?style=for-the-badge)](#license)

*An evolving open-world RPG adventure featuring exploration, turn-based combat, and a rich fantasy setting.*

---

</div>

## 📖 Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Game World & Maps](#game-world--maps)
- [Characters & Classes](#characters--classes)
- [Combat System](#combat-system)
- [Enemies & Bestiary](#enemies--bestiary)
- [Items & Equipment](#items--equipment)
- [Plugins & Extensions](#plugins--extensions)
- [Project Architecture](#project-architecture)
- [Technology Stack](#technology-stack)
- [Getting Started](#getting-started)
- [How to Play](#how-to-play)
- [Repository Structure](#repository-structure)
- [Configuration & Customization](#configuration--customization)
- [Contributing](#contributing)
- [License](#license)

---

## 🎮 About the Project

**RPG Maker MV — Project I** is a classic-style fantasy RPG game developed using [RPG Maker MV](https://www.rpgmakerweb.com/products/rpg-maker-mv). The project showcases an explorable open world with multiple interconnected regions — from mysterious mazes and enchanted gardens to bustling towns with shops, inns, and guilds.

The game is built on an HTML5 / JavaScript engine powered by **Pixi.js** for 2D WebGL rendering, making it deployable as a desktop application (via NW.js) or directly in the browser. It features a turn-based combat system, customizable character classes, and a rich plugin ecosystem including Yanfly Engine enhancements.

> **Status:** Active development — the project continues to receive iterative updates with new maps, gameplay mechanics, and content.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🗺️ **Open World Exploration** | Traverse an overworld connecting diverse regions — towns, gardens, mazes, and more |
| ⚔️ **Turn-Based Combat** | Classic RPG battle system with physical and magical attacks |
| 🧙 **Dual Skill System** | Magic and Special skill types with elemental affinities |
| 📖 **Enemy Encyclopedia** | In-game bestiary to track and catalog encountered enemies |
| 🏠 **Town Life** | Fully interactive town with shops, an inn, a personal house, and a Hunters Guild |
| 🎨 **Grid-Free Doodads** | Richly decorated environments using Yanfly's Grid-Free Doodads system |
| 🎵 **Full Soundtrack** | Complete BGM, BGS, ME, and SE audio library for immersive gameplay |
| 🖥️ **HD Resolution** | Enhanced 1080×720 resolution via YEP Core Engine |
| 💾 **Save System** | Built-in save/load functionality with alternative save screen |

---

## 🗺️ Game World & Maps

The game world consists of **8 interconnected maps** spanning a rich fantasy landscape:

```
                    ┌──────────────┐
                    │   OverWorld  │
                    │  (Map 005)   │
                    └──────┬───────┘
                           │
          ┌────────────────┼────────────────┐
          │                │                │
   ┌──────┴──────┐  ┌─────┴──────┐  ┌──────┴──────┐
   │    Maze     │  │    Town    │  │  Garden of  │
   │  (Map 001)  │  │  (Map 004) │  │   Hamel     │
   └─────────────┘  └─────┬──────┘  │  (Map 002)  │
                          │         └─────────────┘
              ┌───────────┼───────────┐
              │           │           │
       ┌──────┴──┐  ┌────┴────┐  ┌───┴──────┐
       │ MY_House│  │  Shop   │  │   Inn    │
       │(Map 003)│  │(Map 006)│  │(Map 007) │
       └─────────┘  └─────────┘  └──────────┘
                          │
                   ┌──────┴──────┐
                   │  Hunters    │
                   │   Guild     │
                   │  (Map 008)  │
                   └─────────────┘
```

### Map Details

| Map | Name | Description |
|-----|------|-------------|
| 001 | **Maze** | A challenging labyrinth filled with puzzles and encounters |
| 002 | **Garden of Hamel** | A lush, enchanted garden area with unique flora and atmosphere |
| 003 | **MY_House** | The player's personal home base within the Town |
| 004 | **Town** | The central hub — a bustling settlement with NPCs and services |
| 005 | **OverWorld** | The main world map connecting all major locations |
| 006 | **Shop** | A merchant location within Town for buying and selling goods |
| 007 | **Inn** | A resting place in Town where the player can recover |
| 008 | **Hunters Guild** | A guild hall for accepting quests and bounties |

---

## 🧑‍🤝‍🧑 Characters & Classes

### Playable Characters

| Character | Class | Starting Level | Max Level | Note |
|-----------|-------|:--------------:|:---------:|------|
| **Wanderer** | AllRounder | 1 | 99 | The main protagonist — a versatile adventurer |
| **Maria** *(The Witch)* | Mage | 1 | 99 | A powerful spellcaster who joins the party |

### Class System

The game features **5 distinct character classes**, each with unique stat growth curves and abilities:

| Class | Role | Description |
|-------|------|-------------|
| 🛡️ **Hero** | Balanced | The quintessential all-purpose warrior-leader |
| ⚔️ **Warrior** | Physical DPS | Excels in melee combat with high attack power |
| 🔮 **Mage** | Magic DPS | Commands devastating elemental magic spells |
| ✝️ **Priest** | Healer/Support | Specializes in healing and protective magic |
| 🎯 **AllRounder** | Hybrid | Jack-of-all-trades with access to varied abilities |

---

## ⚔️ Combat System

The game uses a **classic turn-based battle system** with the following elements:

### Elemental Affinities

| Element | Icon | Type |
|---------|:----:|------|
| Physical | 💪 | Standard melee/ranged damage |
| Fire | 🔥 | Burning elemental magic |
| Ice | ❄️ | Freezing elemental magic |
| Thunder | ⚡ | Electric elemental magic |
| Water | 🌊 | Aquatic elemental magic |
| Earth | 🪨 | Terra elemental magic |
| Wind | 🌪️ | Aerial elemental magic |
| Light | ✨ | Holy elemental magic |
| Darkness | 🌑 | Shadow elemental magic |

### Skill Types

- **Magic** — Learned magical abilities consuming MP (Fire, Heal, Spark, etc.)
- **Special** — Unique character-specific techniques and abilities

### Core Combat Skills

| Skill | Type | Description |
|-------|------|-------------|
| Attack | Basic | Standard physical attack |
| Guard | Basic | Reduce incoming damage for the turn |
| Dual Attack | Basic | Two consecutive strikes |
| Double Attack | Basic | Enhanced dual strike variant |
| Triple Attack | Basic | Three rapid successive hits |
| Heal | Magic | Restore HP to an ally |
| Fire | Magic | Elemental fire damage to an enemy |
| Spark | Magic | Electric elemental damage |

---

## 👹 Enemies & Bestiary

The game features a diverse roster of enemies with an **in-game Enemy Book** for tracking encounters:

| Enemy | HP | ATK | Threat Level |
|-------|:--:|:---:|:------------:|
| 🦇 **Bat** | 200 | 30 | ★☆☆☆☆ |
| 🟢 **Slime** | 250 | 30 | ★★☆☆☆ |
| 👹 **Orc** | 300 | 30 | ★★☆☆☆ |
| 🐂 **Minotaur** | 500 | 30 | ★★★☆☆ |
| 👿 **Ogre** | 100 | 50 | ★★★★☆ |

> 💡 **Tip:** The Ogre has low HP but compensates with extremely high attack power — prioritize it in battle!

---

## 🎒 Items & Equipment

### Consumable Items

| Item | Effect |
|------|--------|
| 🧪 **Potion** | Restores HP |
| 💧 **Magic Water** | Restores MP |
| 🌿 **Dispel Herb** | Removes negative status effects |
| 💊 **Stimulant** | Boosts combat performance |

### Weapons

| Weapon | Type | Best For |
|--------|------|----------|
| 🗡️ **Sword** | Sword | Warriors, Heroes |
| 🪓 **Axe** | Axe | Warriors, AllRounders |
| 🪄 **Cane** | Cane | Mages, Priests |
| 🏹 **Bow** | Bow | Ranged attackers |

### Armor & Accessories

| Equipment | Category | Slot |
|-----------|----------|------|
| 🛡️ **Shield** | Small Shield | Off-hand |
| 🎩 **Hat** | General Armor | Head |
| 👘 **Cloth** | General Armor | Body |
| 💍 **Ring** | General Armor | Accessory |

### Equipment Slots

Each character can equip items in **5 slots**: `Weapon` · `Shield` · `Head` · `Body` · `Accessory`

---

## 🔌 Plugins & Extensions

The project leverages **5 active plugins** to enhance the core RPG Maker MV experience:

### Yanfly Engine Plugins

| Plugin | Version | Description |
|--------|:-------:|-------------|
| **YEP_CoreEngine** | v1.28 | The backbone of Yanfly's plugin suite — provides bug fixes, UI enhancements, expanded parameter limits (max gold: 99,999,999), HD resolution support (1080×720), configurable fonts, window colors, and gauge styling. Required for most Yanfly plugins. |
| **YEP_GridFreeDoodads** | v1.08 | Enables placement of grid-free decorative objects (doodads) on maps using an in-game editor. Supports both static and animated doodads from the extensive `img/doodads/` library with categories like furniture, plants, structures, lighting, and world elements. |

### Community & Utility Plugins

| Plugin | Description |
|--------|-------------|
| **Community_Basic** | Essential RPG Maker MV community plugin — controls screen dimensions (816×624 base), rendering mode, cache limits, and dash settings. |
| **MadeWithMv** | Displays a customizable "Made with MV" splash screen on startup with configurable fade-in/out times and wait durations. |
| **EnemyBook** | Adds an in-game enemy encyclopedia/bestiary that displays detailed enemy stats. Unknown enemies display as "??????" until encountered. |

### Additional Plugins (Available but Inactive)

The repository also contains the following plugins in the `js/plugins/` directory, available for activation:

| Plugin | Description |
|--------|-------------|
| **AltMenuScreen** | Provides an alternative main menu layout |
| **AltSaveScreen** | Alternative save/load screen UI |
| **SimpleMsgSideView** | Simplified message display for side-view battles |
| **TitleCommandPosition** | Customizes the position of title screen commands |
| **WeaponSkill** | Links specific skills to weapon types |
| **ItemBook** | In-game item encyclopedia (companion to EnemyBook) |

---

## 🏗️ Project Architecture

The project follows the standard **RPG Maker MV** architecture with a modular JavaScript-based engine:

```
RPG_Maker_MV_Project_I/
│
├── index.html              # 🌐 Main entry point — loads all engine scripts
├── package.json            # 📦 NW.js configuration for desktop deployment
├── Game.rpgproject          # 🎮 RPG Maker MV project file
│
├── js/                     # ⚙️ Engine & Game Logic
│   ├── main.js             #    Application bootstrap
│   ├── plugins.js          #    Plugin loader configuration
│   ├── rpg_core.js         #    Core engine (graphics, input, audio, utilities)
│   ├── rpg_managers.js     #    Data, audio, image, scene, and battle managers
│   ├── rpg_objects.js      #    Game objects (actors, enemies, items, maps, party)
│   ├── rpg_scenes.js       #    Scene management (title, map, battle, menu, etc.)
│   ├── rpg_sprites.js      #    Sprite rendering (characters, battlers, animations)
│   ├── rpg_windows.js      #    UI window system (menus, dialogs, HUD)
│   ├── MyChars.json        #    Custom character data definitions
│   ├── libs/               #    Third-party libraries
│   │   ├── pixi.js         #       Pixi.js v4 — 2D WebGL/Canvas renderer
│   │   ├── pixi-tilemap.js #       Tilemap rendering extension for Pixi
│   │   ├── pixi-picture.js #       Picture/sprite management extension
│   │   ├── fpsmeter.js     #       FPS performance meter
│   │   ├── lz-string.js    #       LZ-based string compression (save data)
│   │   └── iphone-inline-video.browser.js  # iOS video compatibility
│   └── plugins/            #    RPG Maker MV plugins (see Plugins section)
│
├── data/                   # 📊 Game Database (JSON)
│   ├── System.json         #    Global game settings, title, terms
│   ├── Actors.json         #    Character/actor definitions
│   ├── Classes.json        #    Character class stat curves
│   ├── Skills.json         #    Skill/ability definitions
│   ├── Items.json          #    Consumable item data
│   ├── Weapons.json        #    Weapon definitions
│   ├── Armors.json         #    Armor/accessory definitions
│   ├── Enemies.json        #    Enemy stat blocks and behaviors
│   ├── Troops.json         #    Enemy encounter group formations
│   ├── States.json         #    Status effects (poison, sleep, etc.)
│   ├── Animations.json     #    Battle animation sequences
│   ├── Tilesets.json       #    Tileset configurations for maps
│   ├── CommonEvents.json   #    Reusable event sequences
│   ├── MapInfos.json       #    Map metadata and hierarchy
│   ├── Map001–Map008.json  #    Individual map data and events
│   └── Doodads.json        #    Grid-free doodad placement data
│
├── img/                    # 🖼️ Visual Assets
│   ├── animations/         #    Battle animation spritesheets
│   ├── battlebacks1/       #    Battle background — ground layer
│   ├── battlebacks2/       #    Battle background — sky/wall layer
│   ├── characters/         #    Character/NPC sprite sheets (32 sheets)
│   ├── doodads/            #    Grid-free decorative assets (47 subcategories)
│   │   ├── Beds, Chairs, Tables, Shelves/     # Furniture
│   │   ├── Plants/, Rocks/, Water/            # Nature elements
│   │   ├── Doors, Fences, Windows, Wall/      # Structural
│   │   ├── Light/, Light/Animated/            # Lighting effects
│   │   ├── Machines, Tools, Vehicles/         # Mechanical
│   │   ├── Food, Clothes, Pictures, Signs/    # Decorative details
│   │   └── World/Structures, Terrain, Trees/  # Overworld objects
│   ├── enemies/            #    Enemy battle sprites
│   ├── faces/              #    Character portrait graphics
│   ├── parallaxes/         #    Parallax scrolling backgrounds
│   ├── sv_actors/          #    Side-view battle actor sprites
│   ├── sv_enemies/         #    Side-view battle enemy sprites
│   ├── system/             #    System UI graphics (window skins, icons)
│   ├── tilesets/           #    Map tileset images
│   ├── titles1/            #    Title screen backgrounds
│   └── titles2/            #    Title screen frame overlays
│
├── audio/                  # 🎵 Audio Assets
│   ├── bgm/                #    Background music tracks
│   ├── bgs/                #    Background ambient sounds (rain, wind, etc.)
│   ├── me/                 #    Musical effects (fanfares, game over, etc.)
│   └── se/                 #    Sound effects (attacks, menus, items, etc.)
│
├── fonts/                  # 🔤 Custom game fonts
├── icon/                   # 🖼️ Application icon
└── save/                   # 💾 Save data directory
```

### Engine Pipeline

```
index.html
    ↓
pixi.js (WebGL/Canvas Renderer)
    ↓
rpg_core.js → rpg_managers.js → rpg_objects.js
    ↓               ↓                ↓
rpg_scenes.js  rpg_sprites.js  rpg_windows.js
    ↓
plugins.js → [Active Plugins]
    ↓
main.js (Bootstrap & Run)
```

---

## 🛠️ Technology Stack

| Technology | Role | Details |
|------------|------|---------|
| **RPG Maker MV** | Game Engine | Visual game development platform for 2D RPGs |
| **JavaScript (ES5)** | Core Language | ~2.5 MB of game engine and plugin code |
| **Pixi.js v4** | 2D Renderer | WebGL-accelerated 2D rendering with Canvas fallback |
| **HTML5** | Entry Point | Web-based application shell |
| **CSS** | Styling | Custom game font loading |
| **NW.js** | Desktop Runtime | Chromium + Node.js desktop wrapper (via `package.json`) |
| **JSON** | Data Format | All game data (maps, actors, items) stored as JSON |
| **LZ-String** | Compression | Efficient save data compression |
| **FPSMeter** | Performance | Real-time FPS monitoring during development |

---

## 🚀 Getting Started

### Prerequisites

- **RPG Maker MV** (for editing the project in the visual editor)
- **OR** a modern web browser (Chrome, Firefox, Edge) for playing the web build
- **OR** [NW.js](https://nwjs.io/) for running as a standalone desktop application

### Running the Game

#### Option 1: RPG Maker MV Editor
1. Install [RPG Maker MV](https://www.rpgmakerweb.com/products/rpg-maker-mv)
2. Clone this repository:
   ```bash
   git clone https://github.com/AmanK27/RPG_Maker_MV_Project_I.git
   ```
3. Open `Game.rpgproject` in RPG Maker MV
4. Press **F5** or click **Playtest** to run the game

#### Option 2: Web Browser
1. Clone the repository
2. Serve the files using a local HTTP server:
   ```bash
   # Using Python 3
   cd RPG_Maker_MV_Project_I
   python3 -m http.server 8080
   ```
3. Open `http://localhost:8080` in your browser

#### Option 3: NW.js Desktop Build
1. Download [NW.js SDK](https://nwjs.io/) for your platform
2. Place the project files in the NW.js directory
3. Run `nw.exe` (Windows) or the NW.js binary for your OS

---

## 🎮 How to Play

| Action | Keyboard | Alternative |
|--------|----------|-------------|
| Move | Arrow Keys | WASD |
| Confirm / Interact | Enter / Space | Z |
| Cancel / Menu | Escape | X |
| Dash | Hold Shift | — |
| Toggle Full Screen | F4 | — |
| Open Debug Console | F8 | (Dev mode only) |

### Gameplay Tips

1. 🏠 Start by exploring **Town** and visiting the **Hunters Guild** for quests
2. 🛒 Stock up on **Potions** and **Magic Water** at the **Shop** before venturing out
3. 🗺️ Use the **OverWorld** map to travel between major locations
4. 📖 Check your **Enemy Book** to review weaknesses of encountered enemies
5. ⚔️ Watch out for **Ogres** — they hit hard despite their low HP!
6. 🏨 Rest at the **Inn** to fully restore your party's HP and MP

---

## 📁 Repository Structure

### File Statistics

| Category | Files | Description |
|----------|:-----:|-------------|
| Audio (BGM, BGS, ME, SE) | ~500+ | Music and sound effects (`.m4a` + `.ogg` dual formats) |
| Images | ~1,500+ | Sprites, tilesets, doodads, UI assets (`.png`) |
| JavaScript | ~17 | Engine core, plugins, and libraries (`.js`) |
| Data | ~23 | Game database files (`.json`) |
| **Total** | **~2,577** | Complete project files |

### Languages Breakdown

| Language | Size | Percentage |
|----------|------|:----------:|
| JavaScript | 2.5 MB | ~99.9% |
| HTML | 1.6 KB | < 0.1% |
| CSS | 236 B | < 0.1% |

---

## ⚙️ Configuration & Customization

### Display Settings (via YEP_CoreEngine)

| Setting | Value |
|---------|-------|
| Screen Resolution | 1080 × 720 |
| Default Window Size | 816 × 624 |
| Font | GameFont, Verdana, Arial, Courier New |
| Font Size | 28px |
| Window Opacity | 192 / 255 |
| Icon Size | 32 × 32 |

### Game Parameters

| Parameter | Value |
|-----------|-------|
| Max Level | 99 |
| Max Gold | 99,999,999 |
| Currency Unit | G 10 |
| Max Actor HP | 9,999 |
| Max Actor MP | 9,999 |
| Max Actor Stats | 999 |
| Max Enemy HP | 999,999 |
| Locale | en_US |

### Plugin Configuration

Plugin settings can be modified in `js/plugins.js` or through the RPG Maker MV Plugin Manager. Key configurable values include:

- **Screen dimensions** — via Community_Basic and YEP_CoreEngine
- **Doodad rendering** — via YEP_GridFreeDoodads (grid snap, smoothing)
- **Splash screen** — via MadeWithMv (custom images, timing)
- **Enemy Book** — via EnemyBook (unknown data placeholder text)

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch:
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Commit** your changes:
   ```bash
   git commit -m 'Add some amazing feature'
   ```
4. **Push** to the branch:
   ```bash
   git push origin feature/amazing-feature
   ```
5. **Open** a Pull Request

### Contribution Ideas

- 🗺️ Design new maps and dungeons
- 👹 Create new enemies and boss encounters
- 🧙 Add new character classes or skills
- 🔌 Integrate additional community plugins
- 🎨 Create custom tilesets or character sprites
- 📝 Write quest storylines and NPC dialogues

---

## 📜 License

This project contains assets and engine code from **RPG Maker MV** by Kadokawa / Degica. Usage is subject to the [RPG Maker MV EULA](https://www.rpgmakerweb.com/eula). Third-party plugins (Yanfly Engine, etc.) are subject to their respective licenses.

---

## 🙏 Acknowledgments

- **[Kadokawa / Degica](https://www.rpgmakerweb.com/)** — RPG Maker MV engine and default assets
- **[Yanfly](http://yanfly.moe/)** — YEP_CoreEngine and YEP_GridFreeDoodads plugins
- **[Pixi.js](https://pixijs.com/)** — High-performance 2D rendering engine
- **RPG Maker MV Community** — Community_Basic plugin and shared resources
- **[Archeia / Nelderson](https://forums.rpgmakerweb.com/)** — MadeWithMv splash screen plugin

---

<div align="center">

**Made with ❤️ using RPG Maker MV**

*Last Updated: June 2018 · Repository Created: June 23, 2018*

</div>
]]>
