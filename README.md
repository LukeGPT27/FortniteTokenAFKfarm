# Queue Automation

Translucent, animated Windows GUI that automatically queues, idles through a match, detects when it's over, leaves and requeues.

> Unofficial. Not affiliated with or endorsed by Epic Games. Automation can violate a game's terms of service and may lead to account actions. **Use at your own risk.**

## Features
- Auto queue -> AFK -> detect match end -> leave -> requeue loop
- Image-based detection (you capture your own buttons once, works at any resolution)
- Animated, translucent PySide6 interface with live log
- START / STOP, CHECK SCREEN, TEST CLICK SPOT
- F10 emergency stop (or move the mouse into the top-left screen corner)
- Signed license keys (Ed25519) with hardware binding

## Get a key
Keys are free. Join the Discord and message me with your **HWID** (shown on the activation screen):

**Discord:** https://discord.gg/yourserver

## Download
Grab the latest `QueueBot.exe` from the [Releases](../../releases) page.

## Run from source
```bash
pip install -r requirements.txt
python main.py
```
Python 3.10 - 3.12, Windows.

## Setup (once)
1. In-game set your lobby to **Squads + Fill**. Run the game in **Windowed Fullscreen**.
2. Open **SETTINGS**, choose a category, click **CAPTURE** and drag a box around the button:
   - `play` - Play / Ready button in the lobby
   - `ingame` - something only visible during a match (minimap, bus icon)
   - `end` - Leave Match / Confirm / Return to Lobby / Continue buttons (as many as needed)
3. Use **CHECK SCREEN** and **TEST CLICK SPOT** to verify, then **START**.

If buttons aren't found, lower *Match confidence* to ~0.7 or re-capture tighter.

## Stop
`F10`, the STOP button, or slam the mouse into the top-left corner.

## Build the exe
```bash
pip install -r requirements.txt
pyinstaller --onefile --windowed --name QueueBot main.py
```

## Notes
- If the game runs as admin, run QueueBot as admin too.
- The license check is a simple access gate for the official build; the source is open.
