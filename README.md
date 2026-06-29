# Adipocere.com — A 1997-2013 Time Capsule

This is a preserved early-internet humor site my friends and I ran back in the day.
It's pure Web 1.0 — hand-crafted HTML from the Netscape Communicator / Word 97 era,
complete with MIDI files, guestbook vibes, and the kind of content that would never
make it past a modern content review board.

## Purpose of this repo

This repo exists so I can learn GitHub Actions CI/CD with a self-hosted runner
on my internal infrastructure. The site itself is static HTML deployed to a
production LAMP server behind a VPN. The deploy pipeline:

1. Push to `main`
2. Self-hosted runner on `lax-admin01` picks up the job
3. Runner rsync's the files to `lax-web01`
4. Old deployment is preserved as `.bak` for instant rollback

It's intentionally simple — no build step, no tests, no database.
Just `git push` → `rsync` → done.

## Contents

- Pure HTML, no frameworks
- JPEG images from 2002-era digital cameras
- MP3 audio files
- A WAV file that will blow your speakers
- The kind of product line that would get you banned from Shopify

## License

This is a historical artifact. It stays as-is.
