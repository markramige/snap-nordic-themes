This is an unofficial Snap release of the [Nordic themes](https://github.com/EliverLara/Nordic).

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-black.svg)](https://snapcraft.io/nordic-themes)

You can install the theme from the Snap Store оr by running:

```
sudo snap install nordic-themes
```
To connect the theme to an app run:
```
sudo snap connect [other snap]:gtk-3-themes nordic-themes:gtk-3-themes
```
To connect the theme to all apps which have available plugs to gtk-common-themes you can run:
```
for i in $(snap connections | grep gtk-common-themes:gtk-3-themes | awk '{print $2}'); do sudo snap connect $i nordic-themes:gtk-3-themes; done
```
