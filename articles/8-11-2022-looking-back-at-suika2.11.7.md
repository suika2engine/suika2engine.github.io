---
layout: article
---

# Suika2.11.6 and 2.11.7

Author: [Kyo](https://github.com/KyouBrayden)

Date: 8th November, 2022

![Suika2.11.7 banner](/images/Suika2.11.7-banner.png)

Hey everyone, it's Kyo. It's been a while since my last update, so we'll be going over some updates from `2.11.6` and the newly released `2.11.7`.

## Bug Fixes and General Changes
A number of bug fixes took place during `2.11.6` and `2.11.7`, some of these include:
* A major fix was made to Suika2.11.6 where `@chs` would cause the application to crash. (`2.11.6`)
* Fixes for Pro and Suika on both platforms
* The Windows application now works with Unicode
* Added Traditional Chinese
* Added French Translation
* Various other updates and changes. See the [pull request for all other minor changes](https://github.com/suika2engine/suika2/pull/95)

## Improved Multilinguilisation

This update brings about a general improvement of support for multilingualisation. These improvements and changes include:
* The user's system locale now determines the language of the interface and story
* The `i18n` config was removed (Internationalisation is always ON)
* `ui.msg.*` config was removed (Built-in multilingualisation)
* Added UI translation (For Pro, only English and Japanese are available)

## Menubars

This update and the improvement of multilingualisation has also allowed for the implementation of menubars on the Mac and Windows distributions of the Suika2 application, something that many people have been hoping for.
For Mac distributions, the menubar will always be displayed; however, as it may be intrusive on Windows distributions, developers can opt to disable the menubar from the `config.txt` file.

On Mac, the menubar can be edited via Xcode when building from source. Those with the adaquite knowledge may be able to do the same for the Windows distribution when editing or building from the source code.

Thank you for reading the update, I look forward to the next one – Kyo.
