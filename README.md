# GoogleDot-Black

A black cursor theme inspired by Google, built as an Xcursor theme.

- **Name:** GoogleDot-Black
- **Comment:** Black cursor theme inspired on Google
- **Inherits:** `hicolor` (falls back to the default theme for any missing cursor)
- **Format:** Xcursor data version 1.0, prebuilt — no compilation step required

## Contents

```
GoogleDot-Black/
├── cursor.theme
├── index.theme
└── cursors/          # 145 cursors: left_ptr, wait, text, move, resize, dnd, ...
```

## Installation

### 1. Copy the theme

For your user only:

```sh
cp -r GoogleDot-Black ~/.local/share/icons/
# or the legacy location, which some apps still check:
cp -r GoogleDot-Black ~/.icons/
```

For all users:

```sh
sudo cp -r GoogleDot-Black /usr/share/icons/
```

### 2. Apply it

**GNOME (Wayland or X11):**

```sh
gsettings set org.gnome.desktop.interface cursor-theme 'GoogleDot-Black'
```

Or use *GNOME Tweaks → Appearance → Cursor*.

**KDE Plasma:** *System Settings → Appearance → Cursors → GoogleDot-Black*.

**XFCE / LXQt:** *Settings → Mouse and Touchpad → Theme* (or *Appearance*).

**Other X11 setups**, add to `~/.icons/default/index.theme`:

```ini
[Icon Theme]
Inherits=GoogleDot-Black
```

**A single terminal/session**, without changing system settings:

```sh
XCURSOR_THEME=GoogleDot-Black XCURSOR_SIZE=24 some-app
```

Log out and back in (or restart your session) if the theme does not refresh immediately.

## Uninstall

```sh
rm -rf ~/.local/share/icons/GoogleDot-Black ~/.icons/GoogleDot-Black
# or, if installed system-wide:
sudo rm -rf /usr/share/icons/GoogleDot-Black
```

Then pick another cursor theme before removing it.

## License

No license file is included with this theme. All rights reserved by the original author unless a license is added later — feel free to open an issue or PR if you are the author or know the source.
