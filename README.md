# Solarized terminator colors

A color theme for [terminator](http://www.tenshu.net/terminator/) using Ethan Schoonover’s [Solarized color scheme](http://ethanschoonover.com/solarized).

## Repositories
  * This theme as a single repository: [/ghuntley/terminator-solarized](https://github.com/ghuntley/terminator-solarized)
  * The main solarized repository: [/altercation/solarized](https://github.com/altercation/solarized)

## Files
  * `config` -  solarized theme for terminator (by [ghuntley](https://github.com/ghuntley))

## Usage
Install the terminator configuration file:

```bash
git clone https://github.com/ghuntley/terminator-solarized.git
cd terminator-solarized
mkdir -p ~/.config/terminator/
touch ~/.config/terminator/config
# if you want to replace current config:
cp config ~/.config/terminator
# if you want to append current config:
cat config >> ~/.config/terminator/
```

Modify the defaults stanza within the terminator configuration file to select your default(s)

```bash
# other text editors are available (gedit, emacs, etc)
vi ~/.config/terminator/config
```

To configure the default scheme used for new windows/tabs to solarized-light; change:

```ini
[[default]]
# solarized-dark
palette = "#073642:#dc322f:#859900:#b58900:#268bd2:#d33682:#2aa198:#eee8d5:#002b36:#cb4b16:#586e75:#657b83:#839496:#6c71c4:#93a1a1:#fdf6e3"
foreground_color = "#eee8d5"
background_color = "#002b36"
cursor_color = "#eee8d5"
```

To:

```ini
[[default]]
# solarized-light
palette = "#073642:#d30102:#859900:#b58900:#6c71c4:#d33682:#2aa198:#839496:#586e75:#cb4b16:#859900:#b58900:#268bd2:#d33682:#2aa198:#93a1a1"
background_color = "#eee8d5"
cursor_color = "#002b36"
foreground_color = "#002b36"
```

To configure the default scheme used upon launch; change:

```ini
[[default]]
  [[[child1]]]
  type = Terminal
  parent = window0
  profile = default
```

To: 
```ini
[[default]]
[[[child1]]]
  type = Terminal
  parent = window0
  profile = solarized-light
```
## Screenshots

![solarized terminator](https://github.com/ghuntley/terminator-solarized/raw/master/screenshots/terminator-solarized.png)

