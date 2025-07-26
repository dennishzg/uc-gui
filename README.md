# uc-gui

GUI resource pack for the Minecraft plugin [UltraCosmetics](https://www.spigotmc.org/resources/10905/).

- Aseprite source files are in `/aseprite/`.
- Resource pack and GUI textures are in `/resourcepack/`.

---

## 🖼️ Preview

### Main menu

![Main menu](.github/readme-assets/preview-bg_main.png)

### Buy menu (keys, cosmetics etc.)

![Buy menu](.github/readme-assets/preview-bg_buy.png)

## 🛠️ How to use

### Add server resource pack

Edit the `server.properties` file:

```properties
resource-pack=https://github.com/dennishzg/uc-gui/releases/download/v1.1.0/UC-GUI-v1.1.0.zip
```

### Create menu

Example menu using DeluxeMenus.

#### GUI texture

- 🏠 = Main menu texture
- 🪙 = Buy menu texture

```yaml
size: 54
menu_title: "&f🎲🎲🎲🎲🎲🎲🎲🎲🏠"
```

#### Custom items

Example:

```text
/minecraft:give @p minecraft:brick[minecraft:item_model="ucgui:uc_items/key"]
```

| Image                         | Item model                 | Description |
| ----------------------------- | -------------------------- | ----------- |
| invisible                     | `ucgui:guis/invisibleitem` | Invisible items are necessary to make the buttons/icons in the GUI clickable. |
| ![Key][p-key]                 | `ucgui:uc_items/key`       | Treasure chest key |

[p-key]: .github/readme-assets/preview-key.png
