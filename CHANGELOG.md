# Changelog

## 1.0.3 — 2026-10-27

- Video Club: a small heading above the posters shows when titles were added: Today, 1 day ago, 2 days ago,
  This week, 2 weeks ago, 1 month ago, 1 year ago and so on (newest in amber). The detail panel shows the date too.
- Video Club search: titles matching your search come first as before, and now the newest releases come first
  within them.
- Live TV search: channel results and guide results show as two separate lists at the same time. In the results,
  ▶ or ▶▶ jumps to the other list and ◀◀ goes back; each list keeps its place.
- Search keyboard: bigger keys and bigger, bolder letters, easier to read from the couch.

## 1.0.2 — 2026-10-24

- Check for updates: the first time, the page lists the exact Fire TV steps to allow updates (Developer options →
  Install unknown apps → TazTv STB → On) and installs by itself when you come back. Only needed once.
- Check for updates shows each release-note item in full.
- Check for updates always opens a fresh Fire TV Install screen (it could bring back the old "App installed." screen
  from a previous update instead).

## 1.0.1 — 2026-10-24

- New **Settings → Check for updates**: downloads the newest version from GitHub and installs it over the old one
  (your portal, favourites and settings stay). It also checks once a day and shows a note on Home when an update
  is out (can be turned off). Only GitHub is contacted.
- Subtitles on a movie with none: Quick Actions shows "None in this stream"; pressing it shows a short message that
  clears after 3 seconds (it used to stay on screen with the info bar).
- Quick Actions: the colour-key dots stay, without the "was" label.
- Guide ☰: "Find in this category" is now **Search all live TV** (every channel; ▶❚❚ still searches the current category).
- **Google TV and other remotes** (no ☰, ▶❚❚, ◀◀ ▶▶): detected automatically. In movies Select pauses, ◀ ▶ rewind / forward,
  ▼ opens Quick Actions; in live TV ◀ ▶ open Quick Actions; in the guide Hold Select opens the actions bar (with −2 h / +2 h).
  Fire TV remote keys are unchanged. Show categories: Hold Select shows / hides all.
- Continue Watching: the detail button is now **Remove all from Continue Watching** (press Select twice);
  Hold Select still removes one title.
- New **Settings → Remote control**: shows the detected remote and lets you choose **Fire TV remote** or **Google / other remote** (any remote without those keys).

## 1.0.0 — 2026-10-23

First public release of **TazTv STB**, an IPTV client for Amazon Fire TV for Stalker / MAG portals
(portal URL + MAC), built to replace STBEmu with a 10-foot TV interface that works with the Fire TV remote only.

App ID `com.taztv.stb.public`. On first run it opens Portal settings with a blank portal URL and MAC: enter the
portal URL, press **Random MAC** and give that MAC to your provider to register (or copy your STBEmu values under
"Moving from STBEmu").

### Remote and navigation
- Everything works with the Fire TV remote only: D-pad, Select, Hold Select, Back, Menu (☰), Play/Pause, Rewind, Fast-forward.
  No colour keys, number keys, phone or voice needed.
- The MAG colour keys are replaced by a ☰ Quick Actions sheet.
- Focus is always visible (amber ring); text sized for reading from the couch.
- Exit from Home closes the app; Settings → Restart app gives a full fresh start.

### Home
- Three colour tiles (Live TV, Video Club, Settings) with a category pop-up above the focused tile.
- Resume strip for the last channel watched (▶❚❚ resumes).
- Account expiry date in the header, amber from 14 days left, red from 3 days; read at startup only.
- Notice after an unexpected close, with details in Health & usage.

### Live TV
- Guide grid: 30-minute slots, 2-hour window, NOW line, muted live preview of the focused channel.
- ▲▼ keeps the programme on now in focus from channel to channel.
- Favourites (Hold Select), sort by number or name, ±2 h jumps, retries for guide info that fails to load.
- Missing logos, numbers or guide info degrade gracefully; channels always play.
- Catch-up (Restart programme) on channels that support it.

### Player
- Info bar with LIVE badge, programme, progress and NEXT; channel up/down within the category.
- Video Club seeking: 10 s jumps that add up and speed up when held, with a seek badge and live preview of the position.
- Big Paused badge; audio track, subtitles, aspect ratio, sleep timer and stream info in Quick Actions.
- Audio and subtitle language remembered across streams.
- Fresh stream link for every play and one automatic retry on errors.

### Video Club
- Poster grid of 3 rows × 6 with the title under each poster and a detail panel (description, director, cast).
- Endless scrolling; posters load once you stop scrolling for half a second (fewer portal requests).
- ALL category, plus Continue Watching with Resume / Start over, and Hold Select to remove a title.
- Series: latest season and episode on top, scrolling season list, ✓ Watched and part-watched progress per episode,
  "6/10 watched" per season; under 1 minute counts as unwatched.

### Search
- On-screen keyboard (◀◀ delete, ▶▶ space, ☰ clear), live results, scroll bar and "n of N results".
- Global search, including hidden categories; adult content never appears in search.
- Live TV search starts at 3 letters to limit portal load.

### Settings
- **Show categories:** choose which Live TV and Video Club categories appear on Home (ALL / All channels still include them).
- **Parental PIN:** adult categories flagged by the portal ask for a PIN (default 0000, change it here); adult content
  is kept out of All channels, ALL, Favourites and search.
- **Portal settings:** "New box" (Random MAC) or "Moving from STBEmu" (MAC, STB model drop-down with MAG250 default,
  serial, device IDs, signature). The working portal path is remembered.
- **Health & usage:** live portal request monitor, 7-day history, problems, playback quality, crashes and device info,
  kept on the TV across restarts; clear cache / clear log.
- **Diagnostics:** step-by-step portal checks and test playback.
- Fire TV screensaver only on Home and Settings, never while watching, browsing or on the guide.

### Privacy
- Portal URL and MAC stay on the TV (app-private storage, backup disabled).
- Logs and the health log never contain the MAC, tokens, account fields or full stream URLs.
