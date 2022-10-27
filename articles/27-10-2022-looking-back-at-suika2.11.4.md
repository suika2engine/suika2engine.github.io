---
layout: article
---

# Looking Back at Suika2.11.4

Author: [Kyo](https://github.com/KyouBrayden)

Date: 27th October, 2022

Hey everyone, it's Kyo again, I hope you've all been having a fantastic week.

This is the first of a somewhat-weekly run-down on Suika2 and its development, so please check back each Friday for a brief overview of the latest regarding the engine.

Today, I'm going to go over some awesome new changes that came in with Suika version `2.11.4`.

## Bug Fixes
A number of bug fixes took place during `2.11.4`, some of these include:
* Fixed window title (Bug: After loading save data, the window title was not updated correctly)
* Fix null pointer reference (for Linux, Android)
* Add missing symbolic links for Android app
* Fixed OpenType font issue

## Video Playback on Mac and Linux
Suika2 has notabely lacked video playback for both macOS and Linux, however, [Kei](https://github.com/ktabata) has been hard at work and these platforms now have the ability to play videos called from scripts!

To play video on these platforms, we recommend storing video in the `.mp4` format, but you can also use the QuickTime File Format (`.mov` and `.qt`) on macOS. This isn't just exciting for macOS-Linux compatibility, but also the future of compatibility with Windows distributions of Suika2.
While not confirmed, the Team have discussed possibliy supporting `.mp4` on the Windows platform when Windows 8.1 reaches its EOL, if this goes ahead, developers will be able to write their scripts universally across the three major platforms – check back in the future to see how this idea is progressing!

## Release Mode and an Independent Linux Packager
Suika2 now supports 'Release Mode', this changes the save directory based on the platform (`AppData` on Windows and `Library` on macOS). This options is, of course, optional and you can toggle it from `conf/config.txt`.

As Suika2 Pro for Creators isn't supported on Linux distributions, an independent Linux packager has been implemented.

Please see [this section](https://github.com/suika2engine/suika2/wiki/6.-Suika2-Pro-for-Creators#export) for instructions.

## NVL-Type Style Support
Suika2 is getting closer-and-closer to supporting NVL, but for now, you can utilise `\n` at the end of lines to make a break.
Combine this with a large (or full screen) message box (either with transparency or a solid colour), altered or removed namebox, and altered margins, you can create a near-perfect allusion of true NVL!

Well, that's all the major stuff for now. I hope you're as excited for the next release as I am!
Have a fantastic week, and I'll see you next Friday!
