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

## Directory structure

Follow
[this page](http://godotengine.org/projects/godot-engine/wiki/Version_Control_and_Project_Organization)
as for directory structure.

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
