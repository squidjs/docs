---
id: configuration
title: Configuring
sidebar_label: Configuration
slug: /customization
---

The configuration file is a [JSON](https://en.wikipedia.org/wiki/JSON) file.
It is located at your user's home directory and called `.squidrc.json`.

## Customizing it
You can easily customize the appearence and features of Squid with its configuration.
When saving the configuration file, you won't need to restart the app.
Most the settings applies immediately after saving the file.

:::info
You will get a notification after saving the configuration file, letting you know if there are any errors.
:::

Most of the settings are self-explanatory, but here are an overview of them:
- `theme` The default theme settings. You can spectify the color in HEX (`#F0F0F0`), RGB (`rgb(0, 0, 45)`) or RGBA (`rgba(9, 11, 16, 0.9)`).
- `defaultShell` The default shell to open
- `shells` The list of shells available in the quick menu
- `webGlRendering` Faster rendering method
- `tabsIcons` If you want to have icons to the left of the tabs
- `css` Aditionnal CSS to add to the window
- `cursor` The style can be `block`, `bar` or `underline`
- `backgroundImage` You can use a background image from your computer, or from any url
- `shortcuts` The shortcuts keybinds
- `localSSHHosts` The local SSH Hosts you want to use. Theses are not saved to the cloud, only on your computer
- `cloudUrl` The url of the cloud server where to save SSH Hosts

## Default configuration
Below is the default configuration:
```json
{
  "theme": {
    "background": "rgba(9, 11, 16, 0.9)",
    "border": "#37474F",
    "text": "#6b6b6b",
    "textHover": "#d0d0d0",
    "foreground": "#ECEFF1",
    "cursor": "#82AAFF",
    "cursorAccent": "#000000",
    "selection": "#82AAFF",
    "black": "#000000",
    "red": "#E54B4B",
    "green": "#9ECE58",
    "yellow": "#FAED70",
    "blue": "#396FE2",
    "magenta": "#BB80B3",
    "cyan": "#2DDAFD",
    "white": "#d0d0d0",
    "brightBlack": "#6b6b6b",
    "brightRed": "#FF5370",
    "brightGreen": "#C3E88D",
    "brightYellow": "#FFCB6B",
    "brightBlue": "#82AAFF",
    "brightMagenta": "#C792EA",
    "brightCyan": "#89DDFF",
    "brightWhite": "#ffffff"
  },
  "defaultShell": {
    "name": "Default",
    "path": "/bin/zsh"
  },
  "shells": [
    {
      "name": "ZSH",
      "path": "/bin/zsh"
    },
    {
      "name": "Bash",
      "path": "/bin/bash"
    }
  ],
  "webGlRendering": true,
  "copyOnSelected": true,
  "restoreWindowPosition": true,
  "tabsIcons": true,
  "altClickMoveCursor": true,
  "vibrancy": true,
  "css": "",
  "bell": {
    "enabled": false,
    "sound": ""
  },
  "cursor": {
    "style": "block",
    "blink": true,
    "width": 1
  },
  "font": {
    "size": 14,
    "family": "monospace",
    "weight": "normal",
    "weightBold": "bold",
    "letterSpacing": 0,
    "lineHeight": 1
  },
  "scroll": {
    "sensitivity": 1,
    "fastScrollSensitivity": 5,
    "fastScrollModifier": "shift"
  },
  "backgroundImage": {
    "enabled": false,
    "opacity": 0.5,
    "image": ""
  },
  "shortcuts": [
    {
      "keybinds": "Cmd+Shift+T",
      "action": "terminal:create"
    },
    {
      "keybinds": "Cmd+Shift+W",
      "action": "terminal:close"
    },
    {
      "keybinds": "Cmd+Shift+O",
      "action": "terminal:zoomin"
    },
    {
      "keybinds": "Cmd+Shift+P",
      "action": "terminal:zoomout"
    },
    {
      "keybinds": "Cmd+Shift+L",
      "action": "terminal:left"
    },
    {
      "keybinds": "Cmd+Shift+M",
      "action": "terminal:right"
    }
  ],
  "localSSHHosts": [
    {
      "name": "Default host",
      "host": "hostname",
      "port": 22,
      "username": "root",
      "password": "removeIfNotNeeded",
      "privateKey": "removeIfNotNeeded"
    }
  ],
  "cloudUrl": ""
}
```
