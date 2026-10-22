# 🌍 RegionSelector

**RegionSelector** is an advanced, lightweight, and fully configurable GUI region-selector plugin built for Paper and Spigot Minecraft servers with BungeeCord/Velocity network support.

---

## ✨ Features

- 🎨 **Fully Customizable GUI & Messages:** Easily configure inventory titles, item materials, display names, lore, and chat messages via `config.yml`.
- 🔌 **Proxy Support:** Seamlessly teleports players across proxy networks (BungeeCord/Velocity) using Minecraft's official Plugin Messaging Channel.
- 🔒 **Item Duplication Protection:** Built-in click event handler prevents players from taking items out of the selector menu.
- ⚙️ **Plug-and-Play:** Automatically generates a default `config.yml` on first startup.

---

## 📜 Commands & Permissions

| Command | Description | Permission |
| :--- | :--- | :--- |
| `/servers` | Opens the Region Selector GUI | Default (All Players) |

---

## ⚙️ Configuration (`config.yml`)

```yaml
# RegionSelector v2.0 Configuration

gui-title: "&8Select a Region"

# Chat Messages
messages:
  connecting: "&aConnecting to %server%..."
  server-offline: "&cThis server is currently offline!"
  only-players: "&cOnly players can execute this command!"

servers:
  eu-central:
    slot: 11
    material: "EMERALD_BLOCK"
    name: "&a&lEU CENTRAL"
    lore:
      - "&7Status: &aONLINE"
      - "&7Players: &e142/500"
      - ""
      - "&e► Click to connect!"
    proxy-server-name: "eu-central"

  na-east:
    slot: 13
    material: "LAPIS_BLOCK"
    name: "&b&lNA EAST"
    lore:
      - "&7Status: &aONLINE"
      - "&7Players: &e89/500"
      - ""
      - "&e► Click to connect!"
    proxy-server-name: "na-east"

  na-west:
    slot: 15
    material: "REDSTONE_BLOCK"
    name: "&c&lNA WEST"
    lore:
      - "&7Status: &cOFFLINE"
      - "&7Players: &e0/500"
      - ""
      - "&c► Server offline"
    proxy-server-name: "na-west"
