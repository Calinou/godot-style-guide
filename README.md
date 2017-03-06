# Godot style guide

This is an unofficial style guide for [Godot](https://godotengine.org), a free,
libre and open source game engine.

## Conventions used in this document

- `snake_case` is **like_this**.
- `camelCase` is **likeThis**.
- `PascalCase` is **LikeThis**.
- `UPPER_SNAKE_CASE` is **LIKE_THIS**.

___

## Naming

- Use `UPPER_SNAKE_CASE` for constants.
- Use `snake_case` for variables and functions.
- Use `snake_case` for input map names.
- Use `snake_case` for all file names.
- Use `PascalCase` for node names.
- Use `PascalCase` for classes.

## Functions

- Function arguments should have a space after each comma, like this:

```gdscript
func my_function(a, b, c):
    pass
```

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

- In most cases, you should use `.tscn` scenes and `.tres` resources as those
  are more friendly towards version control systems.

## Directory structure

Follow
[this page](http://docs.godotengine.org/en/stable/tutorials/engine/project_organization.html)
as for directory structure.

## `.gitignore`

If using Git, you should use a `.gitignore` file that ignores certain patterns
from being added to your Git repository. It should be placed at the root of the
game folder. Here's an example that will suit most Godot projects:

```
.import/
.fscache
*~
```

___

# Contributing to this document

Contributions are welcome, feel free to discuss on the
[issues](https://github.com/Calinou/godot-style-guide/issues).

# License

Copyright (c) 2015-2017 Hugo Locurcio and contributors

CC0 1.0 Universal, see [LICENSE.md](LICENSE.md).
