# gtg-flatpak
Flatpak manifest for Getting Thing GNOME

## How to build:
1 - Install [Flatpak](https://flatpak.org/setup/) & flatpak-builder

2 - Add Flathub remote

```bash
flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
```

3 - Install GNOME's runtime

```bash
flatpak install flathub org.gnome.Platform//3.32
```

4 - Clone the repository

```bash
git clone https://github.com/bilelmoussaoui/gtg-flatpak
cd ./gtg-flatpak
``` 

5 - Build & Install GTG's Flatpak package

```bash
flatpak-builder --install app org.gnome.Gtg.json --user
```
