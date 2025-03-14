# AntiRedstone

![Minecraft Version](https://img.shields.io/badge/Minecraft-1.21.1-brightgreen)
![Spigot Compatible](https://img.shields.io/badge/Spigot-Compatible-orange)
![Paper Compatible](https://img.shields.io/badge/Paper-Compatible-blue)

## Overview
AntiRedstone is a Minecraft plugin that blocks redstone components and notifies administrators with exact coordinates when players attempt to use them. Helps prevent server lag and detects potential griefing attempts using redstone mechanisms.

## Features
- **Block All Redstone Components**: Prevents the use of redstone dust, repeaters, comparators, and other components
- **Instant Notifications**: Alerts administrators when violations are detected
- **Exact Coordinates**: Easily locate where players are attempting to use redstone
- **Prevent Server Lag**: Eliminate a common source of lag from complex redstone mechanisms
- **Griefing Detection**: Stop redstone-based griefing mechanisms before they cause damage

## Installation
1. Download the AntiRedstone.jar file from [Releases](https://github.com/hieu200219/AntiRedstone/releases)
2. Place the file in your server's plugins folder
3. Restart your server
4. Configure permissions if needed

## Permissions
- `antiredstone.bypass` - Allows players to use redstone components
- `antiredstone.notify` - Receive notifications when players attempt to use redstone

## Commands
- `/antiredstone reload` - Reload the plugin configuration
- `/antiredstone toggle` - Enable/disable redstone blocking

## Configuration
```yaml
# AntiRedstone Configuration
notifications:
  enabled: true
  format: "&c[AntiRedstone] &f{player} attempted to use {block} at {x}, {y}, {z}"

blocked-items:
  - REDSTONE
  - REDSTONE_TORCH
  - REPEATER
  - COMPARATOR
  - PISTON
  - STICKY_PISTON
  - OBSERVER
  - REDSTONE_BLOCK
  - LEVER
  - BUTTON
