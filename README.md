# Hyperland Cheat Sheet for Arch Linux

A comprehensive keyboard shortcuts reference for Hyperland window manager on Arch Linux, focusing on SUPER key combinations (Cmd key on Mac).

## Table of Contents

- [Installation on Arch Linux](#installation-on-arch-linux)
- [Window Management](#window-management)
- [Workspace Management](#workspace-management)
- [Application Shortcuts](#application-shortcuts)
- [System Control](#system-control)
- [Layout Management](#layout-management)
- [Floating Windows](#floating-windows)
- [Miscellaneous](#miscellaneous)

## Installation on Arch Linux

```bash
# Install Hyperland
sudo pacman -S hyperland

# Optional dependencies for better experience
sudo pacman -S waybar wofi kitty thunar

# Enable and start the display manager (if using SDDM)
sudo systemctl enable sddm
sudo systemctl start sddm
```

## Window Management

| Shortcut | Action |
|----------|--------|
| `SUPER + Q` | Close active window |
| `SUPER + V` | Toggle floating for active window |
| `SUPER + F` | Toggle fullscreen for active window |
| `SUPER + P` | Toggle pseudo tiling for active window |
| `SUPER + J` | Toggle window split |
| `SUPER + Left Arrow` | Move focus to left window |
| `SUPER + Right Arrow` | Move focus to right window |
| `SUPER + Up Arrow` | Move focus to upper window |
| `SUPER + Down Arrow` | Move focus to lower window |
| `SUPER + SHIFT + Left Arrow` | Move window to the left |
| `SUPER + SHIFT + Right Arrow` | Move window to the right |
| `SUPER + SHIFT + Up Arrow` | Move window up |
| `SUPER + SHIFT + Down Arrow` | Move window down |
| `SUPER + CTRL + Left Arrow` | Resize window (shrink width) |
| `SUPER + CTRL + Right Arrow` | Resize window (grow width) |
| `SUPER + CTRL + Up Arrow` | Resize window (shrink height) |
| `SUPER + CTRL + Down Arrow` | Resize window (grow height) |

## Workspace Management

| Shortcut | Action |
|----------|--------|
| `SUPER + 1-0` | Switch to workspace 1-10 |
| `SUPER + SHIFT + 1-0` | Move active window to workspace 1-10 |
| `SUPER + CTRL + Right` | Next workspace |
| `SUPER + CTRL + Left` | Previous workspace |
| `SUPER + TAB` | Switch to last workspace |
| `SUPER + SHIFT + S` | Move window to special workspace (scratchpad) |
| `SUPER + S` | Toggle special workspace |

## Application Shortcuts

| Shortcut | Action |
|----------|--------|
| `SUPER + Return` | Open terminal (kitty) |
| `SUPER + E` | Open file manager (thunar) |
| `SUPER + R` | Open application launcher (wofi) |
| `SUPER + SPACE` | Open application launcher (rofi/wofi) |
| `SUPER + B` | Open web browser |
| `SUPER + SHIFT + SPACE` | Open emoji picker |

## System Control

| Shortcut | Action |
|----------|--------|
| `SUPER + L` | Lock screen |
| `SUPER + SHIFT + E` | Exit Hyperland |
| `SUPER + SHIFT + R` | Reload Hyperland configuration |
| `SUPER + SHIFT + Q` | Force quit application |
| `SUPER + PRINT` | Screenshot full screen |
| `SUPER + SHIFT + PRINT` | Screenshot region |
| `SUPER + ALT + PRINT` | Screenshot active window |

## Layout Management

| Shortcut | Action |
|----------|--------|
| `SUPER + J` | Toggle split direction |
| `SUPER + SHIFT + SPACE` | Toggle between tiled and floating layout |
| `SUPER + D` | Toggle dwindle layout |
| `SUPER + M` | Toggle master layout |
| `SUPER + SHIFT + F` | Toggle fake fullscreen |

## Floating Windows

| Shortcut | Action |
|----------|--------|
| `SUPER + Mouse Left` | Move floating window |
| `SUPER + Mouse Right` | Resize floating window |
| `SUPER + ALT + Left/Right/Up/Down` | Move floating window |
| `SUPER + ALT + SHIFT + Left/Right/Up/Down` | Resize floating window |
| `SUPER + V` | Toggle floating mode |
| `SUPER + SHIFT + V` | Toggle floating for all windows |

## Miscellaneous

| Shortcut | Action |
|----------|--------|
| `SUPER + H` | Show/hide status bar |
| `SUPER + G` | Toggle gaps |
| `SUPER + SHIFT + G` | Toggle outer gaps |
| `SUPER + U` | Toggle always on top |
| `SUPER + SHIFT + U` | Toggle sticky windows |
| `SUPER + I` | Show window information |
| `SUPER + O` | Toggle opacity |

## Configuration Notes

- **SUPER key**: On Mac keyboards, this corresponds to the Cmd (⌘) key
- **Default config location**: `~/.config/hypr/hyprland.conf`
- **Custom keybinds**: Add to your configuration file using `bind` directive
- **Mouse bindings**: Configured with `bindm` directive

## Example Custom Keybind

```bash
# Add to ~/.config/hypr/hyprland.conf
bind = SUPER, C, exec, code  # Open VS Code
bind = SUPER SHIFT, W, exec, firefox  # Open Firefox
```

## Tips for Mac Users

- The SUPER key is your Cmd (⌘) key
- Alt key functions as expected
- Consider remapping Caps Lock to Ctrl for better ergonomics
- Function keys (F1-F12) work as expected when using `fn` modifier

---

*This cheat sheet covers the most commonly used Hyperland shortcuts. For a complete list of available actions and configuration options, refer to the [official Hyperland documentation](https://hyprland.org/).*
