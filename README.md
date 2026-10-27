Daily Verse

A lightweight Windows desktop widget that brings a new **NIV Bible verse** to your screen each day.

Keep the full verse card visible or switch to a clean, transparent **verse-only view**. Move it wherever you like and let it open automatically when you sign in to Windows.

## Features

- Daily NIV verses from Bible Gateway
- Optional automatic opening at Windows sign-in
- Always-on-top option
- Movable, resizable widget with remembered position and settings
- Transparent verse-only view
- Copy a verse with its reference and attribution
- Tray icon for showing, hiding, and managing the widget
- Last loaded verse available when offline

## Requirements

- Windows 10 or Windows 11
- .NET Framework included with Windows
- Internet access to load new daily verses

No account or API key is required.

## Getting started

1. Download and extract the app into a folder you want to keep.
2. Open **Daily Verse.exe**.
3. Drag the heading to position the widget and resize it from the lower-right corner.
4. Open the **three-dot menu** and enable **Open when Windows starts** if you want it to appear automatically at sign-in.

Keep the app in the same folder after enabling startup. If you move it, open it from the new location and enable startup again.

## Controls

| Action | How |
| --- | --- |
| Show only the verse | Select **Verse only** from the three-dot menu |
| Restore the full widget | Right-click the verse and uncheck **Verse only** |
| Move the widget | Drag its heading, or drag the text in verse-only view |
| Keep it above other windows | Enable **Keep above other windows** |
| Copy the current verse | Select **Copy verse** |
| Refresh the verse | Select **Refresh NIV verse** from the menu |
| Hide the widget | Click **X**; it continues running in the tray |
| Show it again | Click its Bible icon near the Windows clock |
| Quit completely | Select **Exit Daily Verse** from the widget or tray menu |

In verse-only view, hover over the text or choose **Verse details and source** to see the reference and attribution. Your view preference is saved for the next launch.

## Daily updates and offline use

The widget checks for a verse at startup, every 30 minutes, and at local midnight. Bible Gateway chooses the daily passage and controls when its feed changes, so its verse date may differ from your local date.

An internet connection is required for new verses. If the connection drops, the last loaded NIV verse remains visible with its saved date, and the widget retries automatically. It does not switch to another translation.

## Build from source

The `source` folder contains the C# code and app icon. Run `Build.ps1` using Windows PowerShell to build `Daily Verse.exe` with the Windows .NET Framework compiler.

No third-party packages are required.

## Storage and privacy

The widget stores its position and preferences in `Daily Verse.widget.json` and its latest verse response in `Daily Verse.niv-cache.json`, beside the executable. The folder must be writable to save these files.

Automatic opening uses a shortcut named `Daily Verse Widget.lnk` in your Windows Startup folder. The app has no account system or analytics; it connects to Bible Gateway to retrieve the daily verse.

## Scripture attribution

Powered by [BibleGateway.com](https://www.biblegateway.com/). The widget uses its [Verse of the Day service](https://classic.biblegateway.com/usage/votd/docs/).

Scripture taken from the Holy Bible, NEW INTERNATIONAL VERSION®, NIV®. Copyright © 1973, 1978, 1984, 2011 by Biblica, Inc.®  All rights reserved worldwide.

The NIV text belongs to its copyright holder. No library of NIV passages is bundled with the app.
