# Idris Syntax Support for Sublime Text 3

## Installation

```bash
cp ./idris.sublime-syntax  ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/
```
Then switch syntax to `Idris`.

## Testing

```bash
while fswatch -1 ./idris.sublime-syntax; do rsync -a ./idris.sublime-syntax ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/; done
```
