# Config for vscode <!-- omit in toc -->

*This repo is for my private vscode config sync.*

## Index <!-- omit in toc -->

+ [Main settings path macOS](#main-settings-path-macos)
+ [On home machine](#on-home-machine)
	+ [Copy into Library](#copy-into-library)
+ [On work machine (mostly source)](#on-work-machine-mostly-source)
	+ [Symlink from originals](#symlink-from-originals)
	+ [Keybindings](#keybindings)
	+ [Settings](#settings)
	+ [Snippets](#snippets)
+ [On every other machine w/o OneDrive](#on-every-other-machine-wo-onedrive)

## Main settings path macOS

```bash
~/Library/Application Support/Code/User

# bash ready
~/Library/Application\ Support/Code/User
```

## On home machine

> *Sync via OneDrive*

### Copy into Library

```bash
cp keybindings.json ~/Library/Application\ Support/Code/User
cp settings.json ~/Library/Application\ Support/Code/User
cp snippets ~/Library/Application\ Support/Code/User
```

## On work machine (mostly source)

> If machine uses a different GitHub account

### Symlink from originals

> With **hardlink!**

### Keybindings

```bash
ln keybindings.json ~/OneDrive/settings-configs/vscode/vsconf
```

### Settings

```bash
ln settings.json ~/OneDrive/settings-configs/vscode/vsconf
```

### Snippets

> Only as copy because you can't softlink a directory.

```bash
cp snippets ~/OneDrive/settings-configs/vscode/vsconf
```

## On every other machine w/o OneDrive

> *Uses github clone*

```bash
git clone https://github.com/cheeezeburgers/vsconf.git
```
