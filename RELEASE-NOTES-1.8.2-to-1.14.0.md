# PLAYNEX: what's new since 1.8.0

**Latest version: 1.14.0.** This covers every release after 1.8.0 (there was no public 1.8.1). Run the new installer over your old version: it upgrades in place and keeps your library and settings.

---

## Highlights

| Area | What you get | Added in |
| --- | --- | --- |
| **Stores and prices** | Search any game and compare official stores and authorised key sellers, cheapest first, with region and currency choice | 1.9.0 to 1.9.2 |
| **Sounds** | Console-style interface sounds with 8 sound packs, plus dedicated login sounds | 1.9.0 to 1.10.1 |
| **Login screen** | 4 login styles, optional PIN with recovery key, auto-lock, `Ctrl+L` | 1.10.0 to 1.10.5 |
| **Interface styles** | Neon Tokyo, Library Sidebar, Studio Light, Studio Dark and Aurora Glass for every screen (the original look stays the default) | 1.11.0 to 1.11.8 |
| **Display size** | Zoom 50% to 200%, `Ctrl +` / `Ctrl -` / `Ctrl 0`, auto-scaling on 1080p / 1440p / 4K | 1.11.9 to 1.13.3 |
| **Logo picker** | 4 controller logos, show or hide the name | 1.12.0 |
| **Admin games** | Games that need administrator rights are tracked correctly; removing a game wipes its data | 1.11.6 |
| **Controller battery** | Per-controller battery icon and percentage | 1.13.0, 1.13.1 |
| **Auto-changing artwork** | Covers, banners, animated logos and icons rotate from SteamGridDB, with pause and one-click rollback | 1.14.0 |

---

## Major features

### Stores and prices (1.9.0, 1.9.1, 1.9.2)
- New **Stores** tab: search a game and see where to buy it, cheapest first, with discount, lowest price ever recorded, and Steam and Metacritic ratings.
- **Region and currency** picker (India, US, UK, Europe, Canada, Australia and more). Steam shows its real local price; other stores publish US dollars and are converted at the day's rate, marked as estimates.
- Stores without a public price feed (Xbox / Microsoft Store, EA app, Ubisoft, Battle.net, GOG, Epic, Steam) get a "search there" button.
- A Library search with no result offers **Find "name" in stores**.
- Banners and covers now fall back through several sources, and games missing a Steam ID in the price feed are matched to Steam by title.
- Store links only open on a fixed list of official store sites.

### Interface sounds and sound packs (1.9.0 to 1.10.1)
- Optional console-style sounds generated inside PLAYNEX (no audio files).
- Eight packs: Launcher, Modern, Cyberpunk, Robotic, Games (8-bit), Memes, Zen and Minimal, each with Preview buttons.
- Dedicated **login sounds**: startup chime, lock, PIN-digit clicks, wrong-PIN buzz and unlock.

### Login screen and lock (1.10.0 to 1.10.5)
- Optional, **off by default**. Four styles you can switch any time: *Who's playing?*, *Lock screen*, *Key art sign in* and *Controller* (press the glowing button for an animated unlock).
- Optional **PIN** (4 to 8 digits) stored only as a salted hash on your PC and never in backups. Five wrong tries pause the keypad. A **recovery key** is shown once when you set the PIN.
- **Auto-lock** after 5, 15, 30 or 60 idle minutes, **Lock now** and `Ctrl+L`.
- The on-screen keypad is hidden until you click "Show on-screen keypad" (or choose to show it by default). Keyboard PIN entry always works.
- No account and nothing online. This is a privacy screen, not file encryption.

### Interface styles (1.11.0 to 1.11.8)
- Complete new looks for every screen (Home, Library, Game details, Stores, Profile, Settings, Controller test, dialogs): **Neon Tokyo**, **Library Sidebar**, **Studio Light**, **Studio Dark** and **Aurora Glass**.
- The original PLAYNEX style stays the default and is unchanged. Choose in Settings > Appearance > Interface style.
- Neon Tokyo and Studio match their approved designs, including the giant outlined game title, tilted covers, hero cards and stats cards.

### Display size and resolution (1.11.9 to 1.13.3)
- **Display size**: zoom 50% to 200% in Settings > Appearance, with slider, +/- and Reset, for every style. Shortcuts: `Ctrl +`, `Ctrl -`, `Ctrl 0`.
- Big screens (1080p, 1440p, 4K) scale up automatically so nothing looks tiny.
- Neon and Studio now use **one zoom level on every screen**, with Home keeping its larger look.

### Logo picker (1.12.0)
- Four controller logos: **Classic**, **Neon Outline**, **Studio Sunrise** and **Glow Dark**, with a switch to hide the PLAYNEX name next to the logo. The choice also changes the window and tray icon.

### Admin games and clean removal (1.11.6)
- Games that need administrator rights are now recognised as running. PLAYNEX follows the program it started and everything it launches.
- PLAYNEX **no longer forces "Run as administrator"**. Windows shows its own prompt only when a game needs it, and nothing is remembered.
- **Removing a game deletes everything saved about it** (playtime, sessions, favourite, notes, artwork, edits, collections), so adding it again is a fresh entry.

### Controller battery (1.13.0, 1.13.1)
- Each connected controller shows its own battery icon and percentage on the top bar and the Controller test page, numbered when you have more than one. Colour goes green, amber, red.
- Bluetooth controllers that report a real percentage show the exact number. Xbox-style controllers report only four levels, so the value is an estimate.
- Wired and 2.4 GHz receivers show "Cable / 2.4G" because Windows does not report a battery for them.
- The Controller test page lists what Windows reported if no battery number is available.

### Auto-changing artwork (1.14.0)
- With your SteamGridDB key, each game cycles through different **covers, banners, logos (including animated GIF/WebP) and icons**, every 30 minutes by default (10 minutes to 12 hours).
- Settings > Integrations: on/off, **Pause**, interval, which types change, animated logos on/off, **Change now** and **Back to default artwork**.
- **Rollback is safe**: each game's original artwork is never deleted. Turning the feature off restores default art everywhere. In a game's Edit window you can pin its art, change it now or restore its default. Custom art you set yourself is never replaced.

---

## Fixes and smaller improvements

**Screenshots and overlay (1.8.2, 1.8.3)**
- Deleted screenshots no longer leave names or black boxes. The list is checked against the files on disk.
- Delete from a tile, or use **Select** mode to delete many at once (only ever inside your Pictures folder).
- Screenshot hotkey is now **F10** (full screen is **F11**).
- The overlay opens on the first press and hands control straight back to the game when closed.
- Game icons are back in Profile > Games and Most played.

**Profile picture (1.8.4, 1.8.5)**
- New picture editor: zoom, drag, **Fit whole image** or **Fill circle**, and **Adjust picture** to edit later. Large images are shrunk automatically.
- Pictures fill the circle exactly in the profile card and top bar.

**Library and artwork (1.8.5)**
- Missing artwork is repaired at start-up after the old data folder was deleted.
- SteamGridDB matches by Steam ID when available; **Test key & fetch artwork** button.
- Uninstalled games no longer stay in the library.

**Other fixes**
- **1.10.3:** "Forgot your PIN?" no longer freezes PLAYNEX.
- **1.10.1:** login glow and Sign in button colours restored.
- **1.10.2:** Controller test page uses the new layout, with LB, RB, LT and RT lighting live.
- **1.11.8:** Stores search has a clear (X) button; Profile > Games name overlap and missing icons fixed.
- **1.12.0:** programs added by file get readable names ("Cyberpunk 2077" instead of "Cyberpunk2077"); background errors are logged instead of risking a crash.

---

## Version-by-version

| Version | Summary |
| --- | --- |
| **1.14.0** | Auto-changing artwork from SteamGridDB with pause and rollback |
| **1.13.3** | Neon / Studio Home restored to its bigger look |
| **1.13.2** | One zoom level on every screen in Neon and Studio |
| **1.13.1** | Wider battery detection, honest "Cable / 2.4G" label, diagnostics line |
| **1.13.0** | Controller battery icon and percentage |
| **1.12.0** | Logo picker, zoom shortcuts, readable game names, safer background errors |
| **1.11.9** | Display size (50% to 200%), default style scales on big screens |
| **1.11.8** | Neon / Studio Profile, Settings, Stores sizing; Stores clear button; Profile > Games fix |
| **1.11.7** | Studio Light rebuilt to the design; new Studio Dark |
| **1.11.6** | Admin-game tracking, no forced administrator, full cleanup on remove |
| **1.11.5** | Neon Tokyo matches the approved design; auto-scale on big screens |
| **1.11.4** | Neon redesigned as Neon Tokyo |
| **1.11.3** | Neon Home banner shown full screen |
| **1.11.2** | Fixed Home regression in the original style; Neon banner shown once |
| **1.11.1** | Neon, Aurora and Studio Home fixes and content |
| **1.11.0** | Four new interface styles |
| **1.10.5** | On-screen keypad hidden until requested, with a default setting |
| **1.10.4** | Controller login digits on one line |
| **1.10.3** | Fixed "Forgot your PIN?" freeze |
| **1.10.2** | New controller layout on the test page |
| **1.10.1** | New gamepad on the Controller login, login sounds, glow fixes |
| **1.10.0** | Login screen, PIN, recovery key, auto-lock |
| **1.9.2** | Store banner fallbacks, title matching, 8 sound packs |
| **1.9.1** | Region and currency, Stores redesign, many more sounds |
| **1.9.0** | Stores tab with price comparison, interface sounds |
| **1.8.5** | Artwork repair, SteamGridDB by Steam ID, uninstalled games hidden |
| **1.8.4** | Profile picture editor |
| **1.8.3** | F10 screenshot key, overlay reliability, icons restored |
| **1.8.2** | Screenshot cleanup, select and delete |

---

## Upgrade notes
- Install the new `PLAYNEX-Setup-<version>.exe` over the old one. Your library, playtime and settings are kept.
- Nothing new is switched on that sends data anywhere. The login screen, phone remote and SteamGridDB features are optional.
- The font look of Neon Tokyo is best with the free Google fonts Syne and DM Sans installed; without them it uses Segoe UI.
- Some features (battery levels, admin-game tracking, 1440p layout) depend on Windows and hardware. Please report anything that behaves differently on your PC.

*PLAYNEX is an independent personal project, not affiliated with or endorsed by any console maker, store or content site. All names and trademarks belong to their owners.*
