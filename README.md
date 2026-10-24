# TazTv STB

An IPTV player for **Amazon Fire TV** for **Stalker / MAG portals** (portal URL + MAC address), designed for the
Fire TV remote: a TV guide, Video Club with series and Continue Watching, search with an on-screen keyboard,
favourites, parental PIN and more. No colour keys, number keys or phone needed.

> TazTv STB does not provide any channels or content. You need your own subscription from an IPTV provider that
> uses a Stalker / MAG portal.

## Install on a Fire TV
1. On the Fire TV: **Settings → My Fire TV → Developer options**, turn on **Install unknown apps** for the
   **Downloader** app (install Downloader from the Amazon Appstore first).
   If Developer options is hidden: Settings → My Fire TV → About, then press Select on the device name 7 times.
2. Open **Downloader** and enter this short link (always the latest version):

   ```
   tinyurl.com/taztvstb
   ```
   Full link: `https://github.com/Taz101021/taztv-stb/releases/latest/download/TazTv-STB.apk`
   Or download it from the [Releases](https://github.com/Taz101021/taztv-stb/releases/latest) page.
3. Install, then open **TazTv STB** from Your Apps & Channels. To add it to the favourites row, highlight it,
   press ☰ and choose **Move to front**.

Also works on Android TV / Google TV boxes (Android 7.1 or later).

## First-time setup
TazTv STB opens on **Portal settings**:
1. Enter your **portal URL** (from your provider).
2. **New box:** press **Random MAC**, then give that MAC address to your provider so they can register it.
   **Moving from STBEmu:** copy the MAC (and, if your provider needs them, the STB model, serial number and
   device IDs) from your STBEmu profile.
3. Press **Save**. Each MAC works on one device at a time.

## Using it
| Key | Does |
|---|---|
| D-pad / Select | Move / open, watch |
| Hold Select | Add to favourites (guide), remove from Continue Watching (Video Club) |
| ☰ Menu | Quick Actions: favourites, audio, subtitles, aspect ratio, sleep timer (replaces the MAG colour keys) |
| ▶❚❚ | Search, resume, pause |
| ◀◀ ▶▶ | Change page / day in lists; seek in movies |
| Back | Close / go back |

Parental PIN: **0000** until you change it in Settings → Parental PIN.

## Changes
See [CHANGELOG.md](CHANGELOG.md).
