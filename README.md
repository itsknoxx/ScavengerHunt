# 🧭 ScavengerHunt

A fully customizable, team based Minecraft scavenger hunt plugin for Paper servers.

ScavengerHunt enables server owners to run organized scavenger hunt events where players form teams, go into a dedicated event world, pick up objectives and then compete to win.

The plugin has interactive menus, staff controls, objective tracking, world management and inventory protection.

## ✨ Features

### 🎮 Team-Based Events
- Create and manage teams for scavenger hunt competitions.
- Set team numbers and player limits.
- Let the players pick their teams.
- Automatically balance teams when supported by the selected assignment mode.
- Track objective progress and identify the winning teams.

### 🖥️ Interactive GUIs
- Player event menu
- Staff administration menu
- Event settings menu
- World generation and management menu
- Team selection and management menus
- Objective tracking and administration menus

GUI text customization: you can edit the menu titles, item names, button descriptions and hover text via messages.yml.

Supports standard Minecraft color codes (&) and RGB hex colors (&#RRGGBB) including Birdflop generated colors.

### 🌍 World Management
- Create a dedicated scavenger hunt world.
- Pick an existing Event World.
- Configure world borders.
- Generate new worlds with random seeds.
- Recover the plugin owned worlds.
- Archive the previous worlds during supported regeneration operations.
- Set a shared starting spawn location.

Existing worlds are intended to be protected from accidental replacement.

### Chunky Integration
ScavengerHunt integrates with Chunky for controlled world pre-generation.

- Initiate pregen from the staff interface.
- Use Chunky to check on generation progress.
- Receive staff notifications when supported pre-generation has completed.

### Inventory Protection
- Scavenger hunt inventory separate from normal survival inventory.
- Back up player inventories prior to participation.
- Carry out regular inventory takes when players leave the event.
- Handle inventory recovery and safety checks.
- Don't allow hunt items to be taken into normal survival gameplay.

###  Event Management
- Prepare and run the scavenger hunt events.
- Run event countdowns.
- Track the objectives and progress of the team.
- Automatically end any hunts that have been completed.
- Announce the results and the winning teams.
- Return players to the configured spawn.

##  Requirements

- A compatible **Paper or Purpur** Minecraft server
- Java version compatible with your server build
- **Chunky** (optional, for world pregeneration)

ScavengerHunt is built for modern Minecraft server versions (Purpur 26.2 and above).

##  Installation

1. Download or build the ScavengerHunt .jar.
2. Put it in your server's plugins folder.
3. Install Chunky if you'd like world pre-generation.
4. Restart your Minecraft server.
5. Open the plugin interface via /hunt.
6. Set up the teams, the event world and the shared starting spawn.

## Commands

| Command | Description |
|---|---|
| `/hunt` | Opens the ScavengerHunt menu |
| `/scavengerhunt` | Alias for `/hunt` |
| `/hunt admin` | Opens the staff administration menu |
| `/hunt setspawn` | Sets the shared event spawn |
| `/hunt tp` | Staff teleport to the event world |
| `/hunt recover confirm` | Confirms supported world recovery |

Further event management functions are available via the in-game GUI.

##  Permissions

| Permission | Description |
|---|---|
| scavengerhunt.admin | Enables staff to manage scavenger hunt events |

Admin rights default to Server Operators.

##  Customizing GUI Text

GUI text is configured in:

`plugins/ScavengerHunt/messages.yml`

You can customise the supported GUI titles, item display names, descriptions and lore without having to touch the Java at all.

### Color formatting

```yaml
example-title: "&6&lScavenger Hunt"
example-button: "&#FFCC33&lJoin Event"
example-description: "&7Click to participate!"
```

Supported formatting includes:

- `&6`, `&a`, `&c`, and other standard color codes
- `&l` for bold text
- `&o` for italic text
- `&r` to reset formatting
- `&#RRGGBB` for custom RGB colors

Use Birdflop to generate RGB color combinations (https://birdflop.com/resources/rgb/).

**Note:** Only the text associated with the plugin's message configuration can be altered via messages.yml.

## 🚀 Hosting an Event

1. Run `/hunt admin`.
2. Select or create the event world.
3. Set the world border and optionally run Chunky pregen.
4. Set the shared event spawn.
5. Set up the teams and event settings.
6. Prepare the objectives.
7. Allow players to join and select their teams.
8. Start the event.
9. Keep an eye on the team's progress until the hunt is complete.

## 🛡️ Data Safety

ScavengerHunt has protective checks in place for world ownership, inventory backups and event transitions.

Always backup your server and player data prior to upgrading the plugin or regenerating an event world.

Don't manually delete your inventory backups or your world recovery files whilst an event is in progress.
---
## 🍯 Nectar Studios

Built as part of the Nectar's Nook Inc. ecosystem.
Focused on performance, simplicity, and clean server experiences.
Join our Discord!
https://discord.com/invite/nectarsnookinc
