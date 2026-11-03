# Offshore

**No ads. No clutter. Take back your Fire TV.**

Offshore is a free home screen for Amazon Fire TV that replaces the ad-filled Amazon home with a calm one that's
yours: your apps in one row, big photo or live video backgrounds that follow the time of day, the weather and
serious alerts, a file manager, music controls and a sleep timer. No sponsored rows, no autoplay, no account, no
tracking, no data sold.

This repository hosts Offshore's releases and the update feed the app checks.

## Download

The latest version is always described in [`offshore/latest.json`](offshore/latest.json), with its download link and
SHA-256 fingerprint:

```
https://offshoreupdates-web.github.io/offshore/latest.json
```

## Install on a Fire TV

1. On the TV: **Settings > My Fire TV > About**, then click the device name 7 times to turn on Developer options.
2. **Settings > My Fire TV > Developer options**: allow apps from unknown sources for the Downloader app.
3. Install the free **Downloader** app from the Amazon Appstore.
4. In Downloader, enter the APK address from `latest.json` and install it.
5. Press Home: Offshore takes over the home screen. The Amazon home stays installed underneath, untouched.

## Works on

Fire TV devices running **Fire OS 7 or 8**, tested on the Fire TV Cube (3rd gen) and the Fire TV Stick 4K Max
(2nd gen). Newer sticks on Amazon's **Vega OS** can't install apps from outside Amazon's store, so Offshore can't run
there. Settings > My Fire TV > About shows which you have.

## Updates

Offshore checks `latest.json` on the schedule you pick (Settings > Updates & about). When a new version is out, the TV
shows "Update available". **Install now** downloads it and checks that it's the real Offshore before Fire TV's own
install prompt appears:

- it comes from this site, over HTTPS
- it matches the SHA-256 fingerprint in `latest.json`
- it's Offshore, signed with the same key as the version you have
- it's newer than what's installed

You press Install once on the TV; your settings are kept. Android also refuses any update signed with a different key.

## Privacy

No account, no ads, no analytics, no data sold. Settings stay on the TV. Every source of information (weather, news,
scores) is named on screen and can be turned off.

## Files here

| File | What it is |
|---|---|
| `offshore/latest.json` | The update feed: newest version, release notes, download link, SHA-256 |
| `offshore/offshore-<version>.apk` | Each release (older ones stay for anyone who needs them) |
