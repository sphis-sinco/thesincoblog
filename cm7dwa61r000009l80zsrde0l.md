---
title: "SAP Devlog: 2/20/2025"
datePublished: Thu Feb 20 2025 22:09:28 GMT+0000 (Coordinated Universal Time)
cuid: cm7dwa61r000009l80zsrde0l
slug: sap-devlog-2202025
tags: devlog, sinco

---

Heya guys!

So, we have gone from 0.0.5-p to 0.0.7-p I'm pretty sure?

Yeah.

So anyway let's summarize the last few days.

So after 0.0.5-p released a bug was brought to my attention.

The game crashed on launch for windows.

So I had to debug that for a day, figured out it was Translations and then I forgot about the project for 3 days I guess? I was working on some other stuff and just didn't work on the game until 3 days later.

Then we had 0.0.6-p with Removed translations.

But I wasn't a fan of that, I wanted Translations in the game. So for 0.0.7-p I did this complicated-ish system for that and it worked!

Get asset translating working and boom 0.0.7-p could've been done. But **Nah**, I wanted to do more, so I translated the credits, DJ helping with Portuguese as expected, did some credit state modifications and did a bunch of build directory stuff.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1740088769316/e374057a-acfd-4f37-81ff-f7165de8806a.png align="left")

That was fun but doing all this building and changing build flags can be time consuming, but im a programmer, I can fix this, so I made `Build.py`

And it's basically a haxe project compiler using lime with support for custom build flags and trace log copy paste, just a QOL python application using tkinter. Which I'm still updating when I can, lol.

And that's our devlog for today!

Have a good day!