# Idris Syntax Support for Sublime Text 4

Syntax highlighting for Idris and Idris2 source files. The syntax definition
tracks Idris2 language tokens through v0.8.0, including current keywords,
pragmas, nested comments, raw and multiline strings, interpolation, and
underscored numeric literals.

## Installation

```bash
mkdir -p ~/Library/Application\ Support/Sublime\ Text/Packages/IdrisSyntax
cp ./idris.sublime-syntax ~/Library/Application\ Support/Sublime\ Text/Packages/IdrisSyntax/
cp ./Comments.tmPreferences ~/Library/Application\ Support/Sublime\ Text/Packages/IdrisSyntax/
```
Then switch syntax to `Idris`.

## Testing

```bash
while fswatch -1 ./idris.sublime-syntax; do rsync -a ./idris.sublime-syntax ~/Library/Application\ Support/Sublime\ Text/Packages/IdrisSyntax/; done
```
