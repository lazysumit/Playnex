# PLAYNEX Remote (phone control)

Control your PC from your Android phone: see which game is running, take a screenshot, control the music, quit the game, and shut down or restart the PC.

PLAYNEX Remote is a web app that your own PC serves. There is nothing to install from a store: you open it in your phone's browser and add it to the home screen, where it looks and opens like an app.

## Set it up (2 minutes)

1. On the PC, open **PLAYNEX → Settings → Remote** and turn on **Allow my phone to connect**.
2. If Windows asks about the firewall, allow PLAYNEX on **Private networks**.
3. On the same Wi-Fi, open the address shown under **Address** (for example `http://192.168.x.x:47600`) in Chrome on your phone.
4. On the PC press **Pair a phone**. Type the 6-digit code on your phone and press **Connect**.
5. In Chrome choose the menu (three dots), then **Add to Home screen**. PLAYNEX now has its own icon.

## What you can do

| Card | What it does |
| --- | --- |
| Now playing | The game that is running, how long you have played, and a **Quit** button |
| Screenshot | Takes a screenshot of the PC screen and shows it on your phone. You can save it. A copy is also kept on the PC |
| Music | Previous, play / pause and next for the music app on the PC |
| PC | CPU, memory and GPU load |
| Power | **Restart** and **Shut down** with a 10-second countdown you can cancel |

The same Shut down and Restart buttons are on the PC under **Settings → Remote → Power**.

## Using it away from home

The remote only works on your own network by default. To use it when you are away, use a private VPN such as [Tailscale](https://tailscale.com) (free for personal use): install it on the PC and the phone, then open `http://<the PC's Tailscale address>:47600` on the phone. The address appears in the **Address** list in PLAYNEX.

**Do not forward the port on your router.** That would expose your PC to the whole internet. A VPN keeps it private and encrypts the connection.

## Security

- **Off by default.** Nothing listens until you turn it on.
- **One-time pairing code.** It lasts 3 minutes and works once. Five wrong codes lock pairing for 5 minutes.
- **Secret token per phone.** Every request needs it. PLAYNEX stores only a hash of the token, never the token.
- **Remove a phone any time** under Settings → Remote → Paired phones. It loses access straight away.
- **Power actions can be turned off** with **Allow shut down and restart from the phone**.
- The phone page is served with a strict content-security policy and can only call this PC.
- Traffic on your home Wi-Fi is not encrypted (plain HTTP), so only use it on networks you trust, or through a VPN.

## Limits

- The PC must be on, and PLAYNEX must be running (it can sit in the tray).
- A PC that is shut down cannot be turned back on from the phone.
- Screenshots of a locked screen or sleeping monitor may fail or come out blank.
- **Force-close open apps** (Settings → Remote → Power) is off by default. With it off, an app with unsaved work can hold up a shut down.
- This is a web app, not a Play Store app.
