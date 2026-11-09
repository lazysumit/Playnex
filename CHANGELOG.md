# Changelog

All notable changes to PLAYNEX. Newest first.

## 1.7.0
- **Renamed to PLAYNEX** with the tagline *EVERY GAME. ONE DESTINATION*. The app, installer (`PLAYNEX-Setup-<version>.exe`), window title, tray, overlay, shortcuts and docs all use the new name.
- **Added:** PLAYNEX wordmark in the top bar and the tagline in Settings, About.
- **Kept your data:** on first start the new version copies the library, settings and artwork from the old "Game Launcher" data folder, and renames the old screenshots folder, so nothing is lost.
- **Changed:** the installer's file description is now just the tagline.

## 1.6.4
- **Fixed:** with *Keep downloaded pictures* on, the screensaver got stuck on the last picture once the limit was reached.
- **Changed:** the saved pictures now roll. At the limit, every new picture is downloaded fresh and the oldest saved one is deleted. Saved pictures are only replayed when you are offline or the sources can't be reached.

## 1.6.3
- **Added:** *Open folder* button for the screensaver pictures, and the exact folder path is shown in Settings.

## 1.6.2
- **Added:** *Keep downloaded pictures* toggle. Off (default): pictures are deleted the moment the launcher closes. On: pictures are kept so the screensaver works offline, with a *Keep up to* limit (20, 40 or 80).
- **Added:** the screensaver falls back to pictures already on the PC when offline.
- **Fixed:** the privacy check wrongly failed the build because of a third-party e-mail address inside `package-lock.json`. That file is now checked only for the builder's own details and paths.

## 1.6.1
- **Changed:** online wallpapers are fetched **one at a time** while the screensaver plays, not in bulk.
- **Added:** privacy guard. `tools/privacy-check.js` scans the project before the build and the finished installer after it, and deletes the installer if it finds personal or computer details.
- **Added:** `.npmrc` and a quieter install in `build-windows.bat`; the installer name now follows `package.json`.

## 1.6.0
- **Added:** online wallpapers for the screensaver from Wallhaven, Bing daily photos, WallpaperCave and Wallhalla. 16:9 only, at 2K or 4K, in the topics you choose (gaming, nature, animals; optionally space, cars and cities).
- **Added:** switch between online pictures, Library game banners, or a mix.
- **Added:** picture caption (title, source, resolution) and music card placement that avoids it.

## 1.5.5
- **Changed:** Screensaver now has its own tab in Settings instead of sitting under Library.

## 1.5.4
- **Fixed:** rating tiles overlapping in narrow windows.
- **Fixed:** ratings and game names overlapping in the ratings lookup window.

## 1.5.0 – 1.5.3
- **Added:** **GPU usage** in the in-game overlay, next to CPU and RAM.
- **Added:** **ratings and reviews** from Metacritic, Steam and RAWG, with a lookup by game name.
- **Added:** Metacritic headline card on the left of the game page, with a tile for every platform on the right that fills the space (PC highlighted as "Your version").
- **Added:** critic and user reviews from Metacritic, so reviews work without a Steam key.
- **Added:** modern ratings lookup window with a search box and recent searches.
- **Fixed:** the rating ring was clipped and the number sat off-centre; platform tiles are now laid out to use the whole panel.

## 1.0 – 1.4 (foundation)
- Console-style interface: Home, Library, Game details, Gaming profile.
- Game detection for Steam, Epic, Xbox / Game Pass, Ubisoft Connect, EA app, Battle.net, GOG, Riot and Rockstar, plus scanned folders and custom executables.
- Artwork and metadata, playtime and session tracking, achievements, favourites and collections.
- Themes (dark, light, system, colour themes), controller support with a test page, keyboard shortcuts, system tray, notifications.
- Idle screensaver with clock, library showcase, trophies, glass effect, hidden-games toggle.
- Music-app detection with a top-bar icon and now-playing card.
- In-game overlay (`Ctrl+Shift+G`) and screenshot hotkey.
- Windows installer (NSIS) and a GitHub Actions workflow to build it.
