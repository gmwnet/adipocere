# Adipocere.com — A 1997-2013 Time Capsule (100% a Gag Site)

**THIS SITE IS A JOKE. IT IS NOT REAL. IT WAS NEVER REAL.**

If you're reading this and wondering if the products, services, or credit card
numbers on this site are legitimate — they are not. Every single thing on this
site was invented by a group of friends in the late 90s / early 2000s trying
to make each other laugh. The credit card numbers are fake. The products are
fake. The testimonials are fake. The entire thing is a meticulously preserved
early-internet shitpost.

People have apparently contacted the webmaster over the years thinking this is
a real business. That is hilarious to us, but also: **please do not send money
to any address listed on this site.** It is not a real company.

## What this actually is

A preserved early-internet humor site from the Netscape Communicator / Word 97
era, complete with MIDI files, guestbook energy, and the kind of content that
would never make it past a modern content moderation bot.

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
- Fake credit card numbers (they are fake, please do not try to use them)
- The kind of product line that would get you banned from Shopify

## License

This is a historical artifact. It stays as-is.
