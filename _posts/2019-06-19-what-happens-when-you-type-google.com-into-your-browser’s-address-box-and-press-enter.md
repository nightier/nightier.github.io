---
title: what happens when you type google.com into your browser’s address box and press enter
date: 2019-06-19 00:06:52
---
This repository is an attempt to answer the age old interview question "What happens when you type google.com into your browser's address box and press enter?"

Except instead of the usual story, we're going to try to answer this question in as much detail as possible. No skipping out on anything.

This is a collaborative process, so dig in and try to help out! There are tons of details missing, just waiting for you to add them! So send us a pull request, please!
## The "g" key is pressed
The following sections explain the physical keyboard actions and the OS interrupts. When you press the key "g" the browser receives the event and the auto-complete functions kick in. Depending on your browser's algorithm and if you are in private/incognito mode or not various suggestions will be presented to you in the dropbox below the URL bar. Most of these algorithms sort and prioritize results based on search history, bookmarks, cookies, and popular searches from the internet as a whole. As you are typing "google.com" many blocks of code run and the suggestions will be refined with each key press. It may even suggest "google.com" before you finish typing it.

## The "enter" key bottoms out
To pick a zero point, let's choose the Enter key on the keyboard hitting the bottom of its range. At this point, an electrical circuit specific to the enter key is closed (either directly or capacitively). This allows a small amount of current to flow into the logic circuitry of the keyboard, which scans the state of each key switch, debounces the electrical noise of the rapid intermittent closure of the switch, and converts it to a keycode integer, in this case 13. The keyboard controller then encodes the keycode for transport to the computer. This is now almost universally over a Universal Serial Bus (USB) or Bluetooth connection, but historically has been over PS/2 or ADB connections.

In the case of the USB keyboard:

    