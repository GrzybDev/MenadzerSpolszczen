# Menadżer Spolszczeń

Menadżer Spolszczeń is the desktop app of [Baza Spolszczeń](https://bazaspolszczen.pl), the catalogue of Polish fan
translations of games. It finds the games installed on your computer, installs the translations that Baza Spolszczeń
offers for them and keeps them up to date. Every change it makes to a game can be undone.

*Po polsku: [README.pl.md](README.pl.md).*

This repository only publishes the app's releases. Its source code lives in
[JustModIt Manager](https://github.com/GrzybDev/JustModIt-Manager).

## Download

Download `MenadzerSpolszczen-win-Setup.exe` from the [latest
release](https://github.com/GrzybDev/MenadzerSpolszczen/releases/latest) and run it. The app installs for your Windows
user, without administrator rights, and then updates itself.

- Requires Windows 10 or 11, 64-bit.
- Releases marked "Pre-release" are early versions; expect rough edges.
- The app and its installer are code-signed by "Open Source Developer, Marek Grzyb".

## What it does

- **Finds your games** in Steam, GOG (GOG Galaxy, offline installers and Heroic) and the Epic Games Store (the Epic
  Games Launcher, Heroic and Legendary) and follows the stores' changes as they happen, without scanning your drives.
- **"Moje gry"** lists the games for which Baza Spolszczeń has a finished translation that fits your copy of the game;
  the **"Katalog"** lets you browse every translation on the site.
- **Installs translations** with one click or automatically, checks that the translation fits your version of the game
  first, and never touches a game that is running or that the store is updating.
- **Lets you choose** when several teams translated the same game; the teams you prefer in the settings decide what is
  installed automatically.
- **Keeps them up to date**: installs new releases of your translations and puts a translation back when a game update
  overwrote it. A translation is never installed automatically into a game that officially offers Polish.
- **Can undo everything**, even offline: the original files are kept (by default in a hidden `.menadzer-spolszczen`
  folder inside the game's folder), and an interrupted install is rolled back after a crash or power loss.
- **Runs quietly** in the system tray, starting with Windows unless you turn that off.
- **Kreator spolszczeń**, for translators in creator mode, builds translation packages from a folder of translated
  files.

## Privacy

The app collects no data about how you use it. It talks only to Baza Spolszczeń (the list of translations, packages and
images), to GitHub (updates of the app) and to the hosts of the images that the site shows. Downloading a package
counts on the translation's page, just like a download from the website.

## Uninstalling

Uninstall the app in Windows Settings, under Apps. Translations you installed stay in your games: to get the original
files back, uninstall the translations in the app first. The app's settings and records stay in
`%LOCALAPPDATA%\BazaSpolszczen\MenadzerSpolszczen`, so reinstalling it picks up where you left off.

## Licence

The app's code is free software under the GNU General Public License, version 3 or later. The names and logos of Baza
Spolszczeń and Menadżer Spolszczeń are not covered by that licence. See [LICENSE.md](LICENSE.md) for the details and
for where to find the source code of each release.
