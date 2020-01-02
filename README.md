# Config for vscode <!-- omit in toc -->

*This repo is for my private vscode config sync.*

## Index <!-- omit in toc -->

+ [Main settings path macOS](#main-settings-path-macos)
+ [Symlink to originals](#symlink-to-originals)
	+ [Keybindings](#keybindings)
	+ [Settings](#settings)
	+ [Snippets](#snippets)

## Main settings path macOS

```bash
/Users/matthiasstarte/Library/Application Support/Code/User

# bash ready
~/Library/Application\ Support/Code/User
```

## Symlink to originals

> With **hardlink!**

### Keybindings

```bash
ln keybindings.json /Users/matthiasstarte/OneDrive/settings-configs/vscode/vsconf
```

### Settings

```bash
ln settings.json /Users/matthiasstarte/OneDrive/settings-configs/vscode/vsconf
```

### Snippets

> Only as copy because you can't softlink a directory.

```bash
cp snippets /Users/matthiasstarte/OneDrive/settings-configs/vscode/vsconf
```
