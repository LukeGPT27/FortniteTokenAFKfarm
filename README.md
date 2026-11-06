# Queue Automation

Free, translucent, animated Windows GUI that automatically queues, idles through a match, detects when it's over, leaves and requeues. No key needed.

> Unofficial. Not affiliated with or endorsed by Epic Games. Automation can violate a game's terms of service and may lead to account actions. **Use at your own risk.**

## Features
- Auto queue -> AFK -> detect match end -> leave -> requeue loop
- Image-based detection (you capture your own buttons once, works at any resolution)
- Animated, translucent PySide6 interface with live log
- START / STOP, CHECK SCREEN, TEST CLICK SPOT
- F10 emergency stop (or move the mouse into the top-left screen corner)

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
Run `build.bat` (or `pyinstaller --onefile --windowed --name QueueBot main.py`).

## Notes
- If the game runs as admin, run QueueBot as admin too.
# Queue Automation

Free, translucent, animated Windows GUI that automatically queues, idles through a match, detects when it's over, leaves and requeues. No key needed.

> Unofficial. Not affiliated with or endorsed by Epic Games. Automation can violate a game's terms of service and may lead to account actions. **Use at your own risk.**

## Features
- Auto queue -> AFK -> detect match end -> leave -> requeue loop
- Image-based detection (you capture your own buttons once, works at any resolution)
- Animated, translucent PySide6 interface with live log
- START / STOP, CHECK SCREEN, TEST CLICK SPOT
- F10 emergency stop (or move the mouse into the top-left screen corner)

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
Run `build.bat` (or `pyinstaller --onefile --windowed --name QueueBot main.py`).

## Notes
- If the game runs as admin, run QueueBot as admin too.

