# Installation on Linux

This page will detail the required packages to setup a development environment on Linux.

Keep in mind though that distribution's packages may get outdated, especially for distros like Debian and we recommend using Flatpak as a development environment to keep a consistent environment across any distro.

This is generally less of an issue if creating a generic GTK application, but GNOME's Adwaita for example evolves pretty quickly and you want to have access to the newest widgets in your application.

That said I also recommend installing the tools for your distro as well to follow along as we will introduce flatpak integration much later in the series.

## Flatpak

1. Install Flatpak
2. Install the GNOME SDK: `flatpak install flathub org.gnome.Sdk//47`
3. Install the Vala SDK: `flatpak install flathub org.freedesktop.Sdk.Extension.vala//24.08`

For Visual Studio Code users we also recommend installing the [Flatpak Extension](https://marketplace.visualstudio.com/items?itemName=bilelmoussaoui.flatpak-vscode)

## Debian/Ubuntu

This also applies to distributions based on Ubuntu, such as Linux Mint, popOS!, ZorinOS and so on.

```sh
sudo apt-get install build-essential valac meson libgtk-4-dev libadwaita-1-dev
```

## Fedora/RedHat

TODO

## Arch Linux

TODO

