# Tmux 3 Syntax for Sublime Text and `bat`

This project provides syntax definition for scripting Tmux configuration.

## What

These are what this project does:

- Syntax highlighting for :file_folder:`tmux.conf`.
- Compatible with Sublime Text 3 and 4.
- Works with `bat` command-line tool.
- Supports syntax of Tmux 3.
- Written in `.sublime-syntax` rather than `.tmLanguage`.
- MIT licensed-free to use, modify and share.

## How

### Install for Sublime Text

![screeshot showing Tmux config for Sublime Text][sublime_screen]

Clone this repository into your :file_folder:`Package/` folder:

```sh
git clone https://github.com/Edditoria/tmux-sublime.git
```

> [!TIP]
> To find the path of :file_folder:`Package/`, click "Preferences" → "Browse Packages" on menu bar of Sublime Text.

Restart Sublime Text if necessary.

### Install for `bat` CLI

![screeshot showing Tmux config for bat CLI][bat_screen]

Clone this repository into your :file_folder:`bat/syntaxes/` directory:

```sh
mkdir -p "$(bat --config-dir)/syntaxes"
cd "$(bat --config-dir)/syntaxes"
git clone https://github.com/Edditoria/tmux-sublime.git

# Parse into a binary cache
bat cache --build
```

## Why

I want to include my :file_folder:`bat.conf` in my dotfiles without licensing concerns. So, I can `bat tmux.conf # with wings` across my machines. Unfortunately I couldn't find any good and safe project on GitHub.

![Fine. I do it myself.][thanos_image]

## Status

- I create it to "show something" on screen using `bat`. The code is definitely over-simplified currently.
- I would maintain usability in Sublime Text. I don't know how far I can go. It depends on user demand: You!
- Please star this project to notify me to support more.
- Open issues for requests and improvements.

Thank you, open source!

[sublime_screen]: ./docs/images/screenshot-Tmux-conf-Sublime-Text.png "screeshot of Tmux.conf for Sublime Text"
[bat_screen]: ./docs/images/screenshot-Tmux-conf-bat.png "screenshot of Tmux.conf for bat CLI"
[thanos_image]: ./docs/images/thanos-fine-ill-do-it-myself.jpg "Fine. I do it myself."
