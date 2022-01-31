# Nativefier Snap

![Example of Nativefier app in the macOS dock](.github/dock-screenshot.png)

You want to make a native-looking wrapper for WhatsApp Web (or any web page).

```bash
nativefier 'web.whatsapp.com'
```

![Walkthrough animation](.github/nativefier-walkthrough.gif)

You're done.

## Introduction

Nativefier is a command-line tool to easily create a “desktop app” for any web site
with minimal fuss. Apps are wrapped by [Electron](https://www.electronjs.org/)
(which uses Chromium under the hood) in an OS executable (`.app`, `.exe`, etc)
usable on Windows, macOS and Linux.

I built this because I grew tired of having to Alt-Tab to my browser and then search
through numerous open tabs when using Messenger or
Whatsapp Web ([HN thread](https://news.ycombinator.com/item?id=10930718)). Nativefier features:

- Automatically retrieval of app icon / name
- Injection of custom JS & CSS
- Many more, see `nativefier --help`

## Installation

[![nativefier](https://snapcraft.io/nativefier/badge.svg)](https://snapcraft.io/nativefier)

Install the snap with `sudo snap install nativefier`

## Usage

To create a desktop app for medium.com, simply `nativefier 'medium.com'`

Nativefier will try to determine the app name, and well as lots of other options.
If desired, these options can be overwritten. For example, to override the name,
`nativefier --name 'My Medium App' 'medium.com'`

**Run `nativefier --help`**
to learn about command-line flags usable to configure your app.

To have high-quality icons used by default for an app/domain, please
contribute to the [icon repository](https://github.com/nativefier/nativefier-icons).
