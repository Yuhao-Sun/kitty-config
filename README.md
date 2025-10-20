# 🐱 Kitty Terminal Configuration

A modern, visually appealing, and efficient configuration for the [Kitty Terminal Emulator](https://sw.kovidgoyal.net/kitty/), optimized for macOS and productivity.  
This setup focuses on **aesthetic themes**, **smooth workflow shortcuts**, and **high readability**.

---

## 📁 File Structure

```
~/.config/kitty/
├── kitty.conf               # Main configuration file
├── session.conf             # Session startup configuration
└── themes/
    └── catppuccin-mocha.conf # Color theme (Catppuccin Mocha)
```

---

## ✨ Features

- 🎨 **Catppuccin Mocha theme** with gradient background and blur  
- 🪄 **Smooth macOS integration** with custom keyboard mappings  
- 🔤 **JetBrainsMono Nerd Font** for rich icons and clean text  
- 🪟 **Dynamic transparency & blur** with quick opacity adjustment  
- 📑 **Tabbed interface** with powerline-style bar  
- 📋 **Clipboard sync** and copy-on-select  
- 💻 **Fine-tuned cursor, margins, and border settings**

---

## ⚙️ Basic Settings

| Setting | Description |
|----------|--------------|
| `shell_integration off` | Disable built-in shell integration |
| `startup_session` | Loads session from `~/.config/kitty/session.conf` |
| `initial_window_width 120c` | Default window width: 120 characters |
| `initial_window_height 35c` | Default window height: 35 characters |
| `font_family` | `JetBrainsMono Nerd Font` |
| `font_size` | `14.0` |
| `background_opacity` | 0.95 (default, adjustable) |
| `background_blur` | Blur intensity: 15 |
| `tab_bar_style` | Powerline with rounded edges |
| `sync_to_monitor` | Synchronize frame rate to monitor refresh |

---

## 🧩 Keyboard Shortcuts

### 🪞 Opacity Control
| Shortcut | Function |
|-----------|-----------|
| `cmd + opt + [` | Decrease opacity by 0.02 |
| `cmd + opt + ]` | Increase opacity by 0.02 |
| `cmd + opt + w` | (Not defined) |
| `cmd + opt + s` | (Not defined) |

### 🗂️ Tab Management
| Shortcut | Function |
|-----------|-----------|
| `cmd + t` | New tab |
| `cmd + w` | Close tab |
| `cmd + shift + ] / [` | Next / Previous tab |
| `right click` | Next tab |
| `ctrl + right click` | Previous tab |

### 🔠 Font Size Control
| Shortcut | Function |
|-----------|-----------|
| `cmd + =` | Increase font size |
| `cmd + -` | Decrease font size |
| `cmd + 0` | Reset to default |

### 🖥️ Window & Mode
| Shortcut | Function |
|-----------|-----------|
| `cmd + opt + f` | Toggle fullscreen |
| `cmd + opt + m` | Toggle maximized window |
| `cmd + shift + p` | Open command palette |

Requires Kitty ≥ v0.32 for the command palette feature

### 📋 Clipboard
| Shortcut | Function |
|-----------|-----------|
| `cmd + c` | Copy to clipboard |
| `cmd + v` | Paste from clipboard |
| `copy_on_select` | Automatically copy on text selection |

---

## 🧠 Additional Tweaks

- **macOS Settings**
  - `macos_option_as_alt both` for better keyboard compatibility  
  - `macos_thicken_font 0.15` for enhanced readability  

- **Scrollback**
  - 10,000 lines of history (`scrollback_lines 10000`)

- **URL Handling**
  - `cmd + click` to open detected URLs (`detect_urls yes`)

- **Visual Polish**
  - `highlight_cursor_line yes`  
  - `active_border_color #F5C2E7`  
  - `hide_window_decorations titlebar-only`

---

## 🧩 Tab Title Template

```bash
tab_title_template "🐾 {index} {title}"
```
Displays a paw emoji 🐾 followed by the tab index and current title

---

## 🧱 Requirements

- [Kitty Terminal](https://sw.kovidgoyal.net/kitty/)
- [JetBrainsMono Nerd Font](https://www.nerdfonts.com/font-downloads)
- [Catppuccin Mocha Theme for Kitty](https://github.com/catppuccin/kitty)

---

## 📦 Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/Yuhao-Sun/kitty-config.git ~/.config/kitty
   ```
2. (Optional) Install the Catppuccin theme:
   ```bash
   git clone https://github.com/catppuccin/kitty.git ~/.config/kitty/themes
   ```
3. Launch Kitty — the configuration will load automatically

---

## 🧰 Customization Tips

- Adjust transparency in real time using `cmd + opt + [` or `]`
- Modify background gradient colors to match your wallpaper
- Add your preferred session setup in `session.conf`
- Disable blur if using solid backgrounds
- For advanced tweaks, refer to `kitty +kitten show-config --default --docs`

---
