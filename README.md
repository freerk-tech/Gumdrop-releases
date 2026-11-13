# Gumdrop test builds

**Every race, one sweet bite.** Gumdrop is a small Windows app that writes a report after each iRacing race: where you started and finished, best lap, pace, consistency, every incident and pit stop by lap, and what the race did to your iRating and Safety Rating.

This page is the test channel: early builds for teammates to try. Expect rough edges, and say what you find.

## Get it

1. Open [Releases](../../releases) and take `Gumdrop.exe` from the newest one.
2. Put it anywhere (a folder of its own is tidy) and double-click it. There is no installer.
3. Windows may say it "protected your PC", because the file is new and not signed. Choose **More info**, then **Run anyway**.

To update, close Gumdrop (tray icon, Exit) and replace the file with the newer one. Your reports are kept.

## Use it

- Leave it running while you race; it sits in the tray. Tray icon > **Start with Windows** if you want it always there.
- When a race ends for you, the report opens on the taskbar without taking focus, with a notification.
- **Copy as text** puts a short version on the clipboard to paste in a chat. **Save as PDF** writes the whole report as one sheet.
- Out of the box it reports official races only. Tick **Also hosted, league and AI races** at the bottom left for the rest.

## Good to know

- It only reads iRacing's live data on your PC. No iRacing login, nothing is sent anywhere.
- Reports are saved in `%APPDATA%\Gumdrop`.
- Right after a race the iRating change is an estimate (marked `~`). The real iRating and Safety Rating fill in when you join another session in the same licence category between 2 minutes and 36 hours later, with Gumdrop running.
- The live data doesn't say which split you were in, so the report doesn't either.
