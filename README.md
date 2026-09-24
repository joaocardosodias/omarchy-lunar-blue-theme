# Lunar Blue for Omarchy

A graphite-dark Omarchy theme with luminous lunar-blue accents, inspired by
the calm, technical color language of [zed.dev](https://zed.dev/).

The theme is original and is not affiliated with or endorsed by Zed Industries.

![Lunar Blue wallpaper](backgrounds/lunar-blue-wanderer.png)

The theme includes seventeen original wallpapers ranging from cinematic space
compositions to manga-inspired solitude and dark surreal scenes.

## Wallpapers

| Wanderer | Eclipse |
| --- | --- |
| ![A solitary figure beneath a blue planet](backgrounds/lunar-blue-wanderer.png) | ![Two figures watching an eclipse](backgrounds/lunar-blue-eclipse.png) |
| **Solar system** | **Ringed world** |
| ![A dark blue solar system](backgrounds/lunar-blue-orbits.png) | ![An astronaut beneath a ringed planet](backgrounds/lunar-blue-rings.png) |
| **Observatory** |  |
| ![A figure inside a planetary observatory](backgrounds/lunar-blue-observatory.png) |  |

### Solitude series

| On the ridge | Wreckage |
| --- | --- |
| ![A solitary explorer on a lunar ridge](backgrounds/lunar-blue-solitude-on-pole.png) | ![A hooded figure resting among blue ruins](backgrounds/lunar-blue-solitude-wreckage.png) |
| **Climb** | **Ether** |
| ![A lone mountaineer climbing through a blue void](backgrounds/lunar-blue-solitude-climb.png) | ![An ethereal figure dissolving into lunar-blue starlight](backgrounds/lunar-blue-solitude-ether.png) |
| **Eyed** |  |
| ![A seated figure beneath a cosmic blue eye](backgrounds/lunar-blue-solitude-eyed.png) |  |

### Miasma series

| Nature of fear | Crowned |
| --- | --- |
| ![A surreal faceless figure illuminated in lunar blue](backgrounds/lunar-blue-miasma-nature-of-fear.png) | ![A veiled crowned figure emerging from deep blue shadow](backgrounds/lunar-blue-miasma-crowned.png) |
| **Omarchy** |  |
| ![A pixel-art Omarchy wordmark in lunar blue](backgrounds/lunar-blue-miasma-omarchy.png) |  |

### Osaka Jade series

| Glowing city | Shaded entrance |
| --- | --- |
| ![A Japanese hillside city glowing in deep lunar blue](backgrounds/lunar-blue-osaka-glowing-city.png) | ![A traditional Japanese entrance beneath blue hanging foliage](backgrounds/lunar-blue-osaka-shaded-entrance.png) |
| **Mountain moon** | **Omarchy** |
| ![Layered blue mountains beneath a rising moon](backgrounds/lunar-blue-osaka-mountain-moon.png) | ![A deep-blue pixel-art Omarchy wordmark](backgrounds/lunar-blue-osaka-omarchy.png) |

## Palette

| Role | Color |
| --- | --- |
| Background | `#121316` |
| Dark background | `#0d0d0f` |
| Raised surface | `#212328` |
| Foreground | `#e8edf5` |
| Muted text | `#818b9d` |
| Primary accent | `#1348dc` |
| Selection | `#1348dc` |
| Soft highlight | `#8ec5ff` |

## Install

```bash
omarchy theme install https://github.com/joaocardosodias/omarchy-lunar-blue-theme.git
```

Because the repository is named `omarchy-lunar-blue-theme`, Omarchy installs
it under the name `lunar-blue` and applies it automatically.

To apply it again later:

```bash
omarchy theme set lunar-blue
```

## Local development

To test a working tree without cloning it again:

```bash
ln -s "$(pwd)" ~/.config/omarchy/themes/lunar-blue
omarchy theme set lunar-blue
```

Remove the symlink when finished:

```bash
unlink ~/.config/omarchy/themes/lunar-blue
```

## Included

- A complete `colors.toml` palette used by Omarchy to generate terminal,
  shell, Hyprland, editor, and application colors.
- A custom `shell.toml` with solid graphite surfaces, vivid blue focus
  states, and fine borders.
- A blue Yaru icon theme preference.
- Seventeen original dark wallpapers with planets, orbits, human silhouettes,
  and Lunar Blue reinterpretations of the Solitude, Miasma, and Osaka Jade
  visual languages.

## Recommended typography

Lunar Blue uses the same typographic roles as Zed's visual language:

- **Lilex Nerd Font Mono** for the Omarchy bar, terminals, and code.
- **iA Writer Quattro S** for summoned Omarchy menus and editorial text.
- **IBM Plex Sans** for application interfaces such as Zed.

On Arch Linux, the packaged dependencies are:

```bash
omarchy pkg add ttf-ibm-plex ttf-lilex-nerd ttf-ia-writer
```

Apply the system and menu roles with:

```bash
omarchy font set "Lilex Nerd Font Mono"
mkdir -p ~/.config/environment.d
printf 'OMARCHY_MENU_FONT="iA Writer Quattro S"\n' > ~/.config/environment.d/90-lunar-blue-fonts.conf
systemctl --user set-environment OMARCHY_MENU_FONT="iA Writer Quattro S"
omarchy restart shell
```

## Requirements

Built and tested against Omarchy 4.0.x's `colors.toml` theme format.
