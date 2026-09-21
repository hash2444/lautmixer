# LautMixer - Setup help

Everything you need to get **LautMixer** running, step by step. If something goes wrong, check *Troubleshooting* at the end.

## What you need

- Windows 10 or Windows 11 (64-bit)
- Windows 10 version 2004 (May 2020) or newer - the process-loopback boost needs it

## Install and start

1. Download **`LautMixer.exe`** from the [Releases page](../../releases) - or directly from the file list of this repository.
2. Put it anywhere you like, for example in its own folder. There is **no installer**.
3. Double-click it.
4. Windows may show a blue **SmartScreen** window ("Windows protected your PC"), because the file is not code-signed. Click **More info**, then **Run anyway**. Your antivirus may also scan the file for a few seconds on the first start.

## First start

1. Play some audio in an app (browser, game, music player). It shows up as a column within a second or two.
2. Drag its slider above 100 % to boost it (the pink zone). Double-click a slider to return to 100 %.
3. Click the window's close button: LautMixer moves to the tray and keeps boosting. Left-click the tray icon to bring it back, right-click -> *Quit* to exit.

## How to use it

- Autostart with Windows: press `Win+R`, type `shell:startup`, and put a shortcut to `LautMixer.exe` there. In the shortcut's *Target* add ` --tray` at the end to start hidden.

## Troubleshooting

**An app is louder/quieter than expected after LautMixer crashed**

While boosting, LautMixer holds the app's own volume at a tiny value and re-amplifies it. If the program is killed in that moment, open the Windows volume mixer and set the app's slider back up, or simply start LautMixer again and move that slider.

**A slider stays at 100 %**

Some apps cannot be captured (for example protected audio or the built-in *System sounds*). Their slider is limited to 100 %.

**Two mixers fight each other**

Only run one LautMixer at a time. If you started it hidden with `--tray`, look for its icon in the tray.

**Nothing happens when I double-click it**

Wait 10-20 seconds on the very first start (antivirus scan / first-time unpacking). If it still does not appear, right-click the file -> *Properties* -> tick *Unblock* -> *OK*, then start it again.

**SmartScreen or my antivirus complains**

The file is unsigned, which triggers warnings for every small tool. Use *More info* -> *Run anyway*. If your antivirus quarantines it, add the folder to its exclusions or re-download.

## Uninstall

Delete the `.exe`. If the program stored settings (see above), delete that folder too.

## Still stuck?

Open an **Issue** on this repository and tell me your Windows / Minecraft version and what you see (a screenshot helps).

---

Made by **dev:#2444** - [github.com/hash2444](https://github.com/hash2444)
