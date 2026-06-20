<p align="center">
  <img src="images/TitleNew.png" alt="FireMysteryBlocks" width="800">
</p>

<p align="center">
  <img alt="Java" src="https://img.shields.io/badge/Java-17%2B-orange">
  <img alt="Minecraft" src="https://img.shields.io/badge/Minecraft-1.16--1.20.1-brightgreen">
  <img alt="Platform" src="https://img.shields.io/badge/Platform-Spigot%20%7C%20Paper-blue">
  <img alt="License" src="https://img.shields.io/github/license/Firestone82/FireMysteryBlocks">
</p>

Minecraft plugin that adds highly configurable mystery blocks — shared objectives that players race to mine for tiered rewards.

## About

FireMysteryBlocks lets server administrators define special blocks as competitive mining objectives. Players mine them to earn rewards based on contribution level, while the plugin tracks miners, caches payouts for offline players, and regenerates blocks over time. Each block has its own YAML config file, so you can run community events, timed races, and grind zones simultaneously with completely independent settings.

<p align="center">
  <img src="images/Showcase.png" alt="Showcase" width="700">
</p>

## Features

<p align="center">
  <img src="images/Features.png" alt="Features" width="700">
</p>

- Per-block YAML configuration with independent tuning
- Tiered multi-stage rewards triggered on mine, destroy, reset, and regeneration
- Leaderboard tracking with configurable reward levels
- Offline reward caching (`$`-prefixed actions) for players not online at payout time
- Progressive block regeneration after inactivity
- Hologram integration: CMI, HolographicDisplays, DecentHolograms, FancyHolograms
- Customizable inventory GUIs via command or block interaction
- PlaceholderAPI support for scoreboards and chat
- Anti-cheat: mine speed detection with enchantment-aware modifiers
- Full destruction history with timestamps
- SQLite by default; optional MySQL via HikariCP

## Requirements

- Java 17+
- Minecraft 1.16–1.20.1
- Spigot or Paper server
- *(Optional)* PlaceholderAPI, CMI, or a supported hologram plugin

## Setup

1. Download the latest release JAR from the [Releases](https://github.com/Firestone82/FireMysteryBlocks/releases) page.
2. Place the JAR into your server's `plugins/` directory.
3. Start (or restart) the server — the plugin generates `plugins/FireMysteryBlocks/config.yml` and the `blocks/` folder on first run.
4. Edit `plugins/FireMysteryBlocks/config.yml` to configure the database, hologram provider, and global settings.
5. Create individual block definition files under `plugins/FireMysteryBlocks/blocks/`.
6. Run `/fmb reload` to apply changes without a server restart.

## Commands

<p align="center">
  <img src="images/Commands.png" alt="Commands" width="700">
</p>

## Permissions

<p align="center">
  <img src="images/Permissions.png" alt="Permissions" width="700">
</p>

Permissions follow the pattern `firemysteryblocks.command.<command>` for commands and `firemysteryblocks.<block>.<action>` for per-block actions.

## PlaceholderAPI

<p align="center">
  <img src="images/Placeholders.png" alt="PlaceholderAPI placeholders" width="700">
</p>

Color codes support gradients via IridiumColorAPI: `<GRADIENT:FF0000>text</GRADIENT:0000FF>`.

## License

MIT License
