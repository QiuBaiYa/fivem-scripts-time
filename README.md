# 🎮 GTA World Style Bottom HUD

> Screen bottom-center HUD displaying Time, Server Name, and Player Count — GTA World style

---

## ✨ Features

- ⏰ **Real-time Clock** — 24h / 12h format, timezone configurable
- 🖥️ **Server Name** — Custom server name display
- 👥 **Player Count** — Live online player count with max capacity
- 🆔 **Server ID** — Shows your own server ID
- 📅 **Date Display** — Optional date with day of week
- 🎮 **Game Time Support** — Can display in-game time instead of real time
- 🎨 **GTA World Classic Style** — Dark semi-transparent bar, clean white text
- ⚡ **Lightweight** — NUI-based, minimal resource usage
- 🔧 **Standalone** — No framework dependency required

---

## Preview

```
┌──────────────────────────────────────────────────────────────┐
│  🕐 14:30 Wed, Jul 9  │  🖥 GTA World  │  👥 Players: 87 / 2048  │  ID: 1  │
└──────────────────────────────────────────────────────────────┘
                          ↑ Bottom center of screen
```

---

## 📦 Installation

### 1. Place the resource
```
resources/
  └── gtaworld-hud/
      ├── fxmanifest.lua
      ├── config.lua
      ├── server.lua
      ├── client.lua
      └── html/
          ├── index.html
          ├── style.css
          └── script.js
```

### 2. Add to server.cfg
```cfg
ensure gtaworld-hud
```

### 3. Restart server

---

## ⚙️ Configuration (`config.lua`)

| Option | Default | Description |
|--------|---------|-------------|
| `Config.ServerName` | `'GTA World'` | Your server name |
| `Config.MaxPlayers` | `200` | Max player capacity |
| `Config.TimeFormat` | `'24h'` | `'24h'` or `'12h'` |
| `Config.UseGameTime` | `false` | Use in-game time instead of real time |
| `Config.TimeZoneOffset` | `8` | UTC offset (China=8, US East=-5, UTC=0) |
| `Config.ShowDate` | `true` | Show date beside time |
| `Config.ShowPlayerCount` | `true` | Show online player count |
| `Config.ShowServerName` | `true` | Show server name |
| `Config.ShowServerID` | `true` | Show your server ID |
| `Config.UpdateInterval` | `5000` | Player count refresh interval (ms) |
| `Config.ToggleCommand` | `'togglehud'` | Command to toggle HUD visibility |

---

## 🎮 In-Game Commands

| Command | Description |
|---------|-------------|
| `/togglehud` | Toggle HUD on/off |

---
<img width="567" height="83" alt="image" src="https://github.com/user-attachments/assets/d52e2b54-061b-4b4f-b54f-b04aa02c67e8" />


## 📄 License
MIT License
