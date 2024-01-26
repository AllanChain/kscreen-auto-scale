# KScreen Auto Scale

Automatically choose and apply scale for external monitors, with KScreen and Wayland.

> [!Warning]
> This project is created for my personal use. If you find it needs improvement, please leave a comment and let's see if we can make it better!

It's better with a desktop shortcut `kscreen-auto-scale.desktop`:

```ini
#!/usr/bin/env xdg-open
[Desktop Entry]
Name=Auto Scale Screen
Exec=/path/to/kscreen-auto-scale/kscreen-auto-scale
Icon=cs-screen
Type=Application
```

## Features

- When only one monitor is connected, reset to preferred mode with proper scale
- When external monitor is connected in extend mode, set both of them to preferred mode with proper scale
- When external monitor is connected in mirror mode, set both of then to 16:9 mode with proper scale

To determine the proper scale, you can pass `--preferred-width` argument. The default value is 1536, which is 1.25x scale with 1920 width.
