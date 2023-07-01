# uc-gui

Resource pack/GUI for the Minecraft plugin [UltraCosmetics](https://github.com/datatags/UltraCosmetics).

- Aseprite source files are in `/aseprite/`.
- Resource pack/GUI textures are in `/resourcepack/`.

---

## 🖼️ Preview

### Main menu

![Main menu](.github/readme-assets/do-not-use-main-menu.png)

### Buy menu (keys, cosmetics etc.)

![Buy menu](.github/readme-assets/do-not-use-buy-menu.png)

### Rename pet

???

## 🛠️ How to use

Example menu using DeluxeMenus.

### GUI texture

- 🏠 = Main menu texture
- 🪙 = Buy menu texture

```yaml
size: 54
menu_title: "&f🎲🎲🎲🎲🎲🎲🎲🎲🏠"
```

### Invisible items

Invisible items are necessary to make the buttons/icons in the GUI clickable. Create an invisible item with:

```yaml
items:
  'test':
    material: MAP
    nbt_int: CustomModelData:1010
    slot: 23
    display_name: "&aInvisible item"
```
