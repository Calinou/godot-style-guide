# Godot style guide

This is an unofficial style guide for [Godot](http://godotengine.org), a free,
libre and open source game engine.

## Conventions used in this document

- `snake_case` is **like_this**.
- `camelCase` is **likeThis**.
- `PascalCase` is **LikeThis**.
- `UPPER_SNAKE_CASE` is **LIKE_THIS**.

___

## Naming

- `UPPER_SNAKE_CASE` for constants.
- `snake_case` for variables and functions.
- `snake_case` for input map names.
- `snake_case` for all file names.
- `PascalCase` for node names.
- `PascalCase` for classes.

## Comments

- Begin comments with an uppercase letter, unless you are referencing a function
  or a variable. Do not end them with a period, unless the comment has several
  sentences.

- Comments should have a space after the `#` symbol, and should be indented as
  usual.

Example:

```gdscript
# Outputs "Hello world!" to console
print("Hello world!")
```

## Indentation

- **Always** use tabs for indentation, GDScript does not like spaces anyway.

## Line lengths

- Try to keep lines under 80 characters. Disregarding this guideline at times is
  acceptable, but over 100 characters is definitely too much.

## Spacing

- Put spaces around operators. Example:

```gdscript
print(str(5 * 40 + 2))
```

## File types and extensions

- Use `.xscn` for text scenes, or `.tscn` when loading will be available.
  (Currently, you can only save `.tscn` scenes, not load them.)
- In general, when developing using a version control system, you should use
  text-based files as much as possible. This is especially true with Git.

## Recommended directory structure

This is an example of an optimal directory structure for working with Godot:

```
├── doc
│   ├── licenses
│   │   ├── cc_by_4.0.md
│   │   ├── cc_by-sa_4.0.md
│   │   └── cc0.md
│   ├── design_document.md
│   └── README.md
├── assets (1)
│   ├── fonts
│   │   └── sourcesanspro
│   │       ├── sourcesanspro_bold.ttf
│   │       └── sourcesanspro_regular.ttf
│   ├── gui
│   ├── locale
│   │   ├── de
│   │   │   └── de.csv
│   │   ├── en
│   │   │   └── en.csv
│   │   ├── es
│   │   │   └── es.csv
│   │   └── fr
│   │       └── fr.csv
│   ├── models
│   ├── music
│   ├── sounds
│   └── textures
├── misc
│   └── tools
│       └── example_python_script.py
├── resources
│   ├── fonts
│   │   └── sourcesanspro
│   │       ├── sourcesanspro_bold.fnt
│   │       └── sourcesanspro_regular.fnt
│   ├── gui
│   ├── locale
│   │   ├── de
│   │   ├── en
│   │   ├── es
│   │   └── fr
│   ├── maps (2)
│   │   └── introduction
│   │       ├── introduction.gd
│   │       ├── introduction.png
│   │       └── introduction.scn
│   ├── materials
│   ├── models
│   ├── music
│   ├── sample_libraries
│   ├── sounds
│   └── textures
├── scenes
│   ├── main_menu.xscn
│   └── player.xscn
├── scripts
│   ├── hud.gd
│   ├── main.gd
│   └── main_menu.gd
├── CHANGELOG.md
├── CONTRIBUTING.md (3)
├── engine.cfg
├── LICENSE.md
└── README.md
```

- (1): `assets` contains the source files of your artwork, like .dae, .csv... It
  should be a separate Git repository or a submodule, unless
  your game is very small. It should not be required to play the project, but is
  a must-have for developing.

- (2): For consistency, it is probably best to name it `maps`, even for a racing
  game or a platformer, where `tracks` or `levels` would have been more
  suitable.

- (3): `CONTRIBUTING.md`, as popularized by GitHub, contains instructions for
  contributing to the project.

## `.gitignore`

You should use a `.gitignore` file that ignores certain patterns from being
added to your Git repository. It should be placed at the root of the game
folder. Here's an example that will suit most Godot projects:

```
bin/
.fscache
*~
```

___

# Contributing to this document

Contributions are welcome, feel free to discuss on the
[issues](https://github.com/Calinou/godot-style-guide/issues).

# License

Copyright (c) 2015 Calinou and contributors  
CC0 1.0 Universal, see [LICENSE.md](LICENSE.md).
