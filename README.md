# Gumdrop test builds

**Every race, one sweet bite.** Gumdrop is a small Windows app that writes a report after each iRacing race: where you started and finished, best lap, pace, consistency, every incident and pit stop by lap, and what the race did to your iRating and Safety Rating.

This page is the test channel: early builds for teammates to try. Expect rough edges, and say what you find.

## Get it

1. Open [Releases](../../releases) and take `Gumdrop.exe` from the newest one.
2. Put it anywhere (a folder of its own is tidy) and double-click it. There is no installer.
3. Windows may say it "protected your PC", because the file is new and not signed. Choose **More info**, then **Run anyway**.

Put it in a folder you can write to (your Desktop, Documents or a folder of your own, not Program Files): Gumdrop updates itself there.

## Updates

From 0.1.1 on, Gumdrop looks for new versions every few hours and shows a card in its window when there is one. Nothing installs until you click **Update now**, and never during a race session. It then downloads the new version, checks it and restarts. Your reports are kept, and the version you had stays next to it as `Gumdrop.previous.exe`.

What an update is checked against: its SHA-256 must match the release's `Gumdrop.exe.sha256` and what GitHub reports for the file, it must be signed with Gumdrop's release key (which never leaves the PC the releases are made on), and it must say it is the version the release says. Windows SmartScreen checks the first `Gumdrop.exe` you download from this page; updates the app downloads itself are not checked by SmartScreen, only by these checks and your antivirus as usual.

## Use it

- Leave it running while you race; it sits in the tray. Tray icon > **Start with Windows** if you want it always there.
- When a race ends for you, the report opens on the taskbar without taking focus, with a notification.
- **Copy as text** puts a short version on the clipboard to paste in a chat. **Save as PDF** writes the whole report as one sheet.
- Out of the box it reports official races only. Tick **Also hosted, league and AI races** at the bottom left for the rest.

## Good to know

- It only reads iRacing's live data on your PC. No iRacing login, nothing about you is sent anywhere. The only thing it asks the internet for is this page's list of releases (and a new version, when you click Update now); you can switch that off with **Check for updates** at the bottom left.
- Reports are saved in `%APPDATA%\Gumdrop`.
- Right after a race the iRating change is an estimate (marked `~`). The real iRating and Safety Rating fill in when you join another session in the same licence category between 2 minutes and 36 hours later, with Gumdrop running.
- The live data doesn't say which split you were in, so the report doesn't either.
