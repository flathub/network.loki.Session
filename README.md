# Session Desktop

This is the Flatpak version of [session-desktop](https://github.com/oxen-io/session-desktop).

## Reporting bugs

If you believe the problem you are experiencing is caused due to the app being a Flatpak or if you only experience it in the Flatpak version and **not** any of the others, please [open an issue here](https://github.com/flathub/network.loki.Session/issues/new).

In any other case, please [report it to upsteam](https://github.com/oxen-io/session-desktop/issues/new/choose) after checking that it [hasn't been reported already](https://github.com/oxen-io/session-desktop/issues).

## Wayland

Wayland support is experimental however you can run Session under it by providing the following flags:

```
flatpak run network.loki.Session --ozone-platform=wayland --enable-features=UseOzonePlatform --enable-features=WaylandWindowDecorations --disable-gpu
```

* `--ozone-platform=wayland`: Use wayland
* `--enable-features=WaylandWindowDecorations`: Add window decorations but will break fullscreen and resizing
* `--disable-gpu`: May be needed
* `--disable-gpu-sandbox`: May be needed on NVIDIA devices
