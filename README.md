# FireMysteryBlocks

Minecraft plugin that adds highly configurable mystery blocks — shared objectives that players race to mine for tiered rewards.

![Java](https://img.shields.io/badge/Java-17%2B-orange) ![Minecraft](https://img.shields.io/badge/Minecraft-1.16--1.20.1-brightgreen) ![Platform](https://img.shields.io/badge/Platform-Spigot%20%7C%20Paper-blue)

## About

FireMysteryBlocks lets server administrators define special blocks that function as competitive mining objectives. Players mine them to earn rewards based on contribution level, while blocks track miners, record history, and regenerate over time. Each block is independently configured via its own YAML file, making it easy to run community events, timed races, and anti-cheat-protected grinding zones simultaneously.

## Features

- Per-block YAML configuration with independent tuning
- Tiered multi-stage rewards triggered on mine, destroy, reset, and regeneration events
- Leaderboard tracking with configurable reward levels
- Offline reward caching for players who are not online at payout time
- Progressive block regeneration after inactivity
- Hologram integration: CMI, HolographicDisplays, DecentHolograms, FancyHolograms
- Customizable inventory GUIs accessible via command or block interaction
- PlaceholderAPI support for scoreboards and chat
- Anti-cheat measures: speed detection and AFK prevention
- History tracking with timestamps

## Requirements

- Java 17+
- Minecraft 1.16–1.20.1
- Spigot or Paper server
- *(Optional)* PlaceholderAPI, CMI, or a supported hologram plugin

## Setup

1. Download the latest release JAR and place it in your server's `plugins/` folder.
2. Restart the server to generate the default configuration.
3. Edit `plugins/FireMysteryBlocks/config.yml` and the per-block files in `plugins/FireMysteryBlocks/blocks/`.
4. Use `/fmb reload` to apply changes without restarting.

## License

MIT License
