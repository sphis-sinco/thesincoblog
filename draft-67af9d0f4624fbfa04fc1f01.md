---
title: "SAP Devlog: 2-15-2025"
slug: sap-devlog-2-15-2025

---

Would you like to help on Sinco and Portilizen?

Fill out this google form: [https://forms.gle/YG4KV71dWmuPRZaA8](https://forms.gle/YG4KV71dWmuPRZaA8).

When it comes to the Pre-Alpha stage of the game I am hoping to give a fun little demo for people to play.

The day before valentine’s day (2/13/2025) I had created an “INDEV ROADMAP” and It starts with the Prototype in February, moving to the Pre-Alpha from February to March. But at the rate I’m going I think the Pre-Alpha might come sooner.

If I had to give a rough estimate I think near the end of February is most likely.

But onto actual work.

# 2-14-2025: Post-devlog

Since I use build flags a lot for development I made a build flags markdown file, with all of the concurrent build flags that I had found to be implemented.

I made the Portilizen Results Screen Assets, and fixed some issues when it came to compiling since I use [Hash Link](https://hashlink.haxe.org) to quickly test my changes without the long wait of compiling for windows.

I then also added a STAGE\_FOUR build flag so I could quickly test the fourth stage when I was working on increasing the size of the countdown text.

After that I worked on the OST Video and now this devlog. I really don’t know what else to add and I’ve been thinking about the Pre-Alpha quite a lot. I’ve been watching a lot of Project Feline devlogs and I’ve been wondering if I should increase the size of the team working on the game. So far it has only been me working with DJ and Paul as they test the builds I release on the private github repo. They’ve given feedback but not enough. Also ComaToast helping me with code.

I’ve been debating on if I should work on mod support using [Polymod](https://polymod.io) but in the past when I’ve tried working with it in the latest version (1.8.0), I’ve come into several bugs with one of the dependencies it uses. And either way the only person who would mod the game is me and I have access to the source code. And when the Pre-Alpha releases, so will the source code. So the Polymod implementation would only work for those who want to mod the game and don’t feel like compiling the game. And either way again I mention the several bugs I’ve come into contact with using the latest version.

So the real question I’ve had for myself is “What should I work on next in preparation for the Pre-Alpha?”

I’ve already got a functional game demo, and the Private TODO Project on GitHub I have for the game only really talks about things I finish quickly anyway besides the settings menu which I don’t know how I could implement that.

I’ve got the idea of making editors for the game, but what can they be for? What can their purpose be? I’ve got the idea of making something soft-coded via JSON data files. In the fourth level I could soft-code the background positions, player and enemy positions. In the first level I could soft-code the same things, but I could also soft-code the `FlxG.random.int(0, 200)` into 2 different JSON values, the health values as well.

Ok, it’s 4:58 PM. I’ve just created a [PR for a Credits menu](https://github.com/sphis-Sinco/SincoAndPortilizen/pull/2) and I’m deciding on if I should stick to this process of making a branch for major changes like a credits menu or a settings menu. But now I’m working on the Credits menu again, working on [scrolling](https://youtu.be/H0_9dSuu0tg). And after I spent awhile on the [scroll limiting](https://github.com/sphis-Sinco/SincoAndPortilizen/commit/e9515f98a83c4f058592b62fbf7e38662cfeb07a). I feel so proud of the credits menu.

I’m watching a Project Feline devlog and it’s talking about a game expansion pack and now I’m thinking about the mod support again and I’m thinking about having DLC content like most games but instead of being the rest of the game I’m thinking of it being fun little bonuses of gameplay. I want v1.0 of Sinco and Portilizen to be the full game (mainly every stage). So having DLC content that just adds one of the stages sounds annoying and tedious, maybe I could work on soft-coding the stages so it would be possible for players but DLC’s that just continue the gameplay, I won’t want that.

From the Pre-Alpha stage to the Beta stage I would like to make SOME levels, but not all. I wanna get up to Stage 6 and v1.0 has stage 7, I wanna work more on the stages but at the same time I don’t… I’m procrastinating… And I’m not liking that.

An HTML build of a game is supposed to be the game on web with maybe some limitations if you want people to buy your game but want them to see your game and check it out before they decide to buy it. But what if the Sinco and Portilizen HTML build was the same except the game is still free? You get to preview the game but you have to download it to play the rest of the content. I’m thinking Stage 1 and Stage 4 can be the HTML Stages. And maybe in the game there can be some bonus content inside the HTML build too.

What if I just, went from Prototype to Alpha instead of Pre-Alpha? Instead of having another era of development to iron out things even more when I’m already doing that, what if I just head straight into the alpha stage? I think it could work.

I’ve thought about the increase in the team size again and I’ve decided to make a [google form to get developers](https://forms.gle/YG4KV71dWmuPRZaA8) willing to play the game without having to ask around.

I’ve thought about Localization, I was gonna try it earlier but then I stopped. The amount of text in the game at the time had scared me out of it. But now I’m thinking about it again, I was and want to use the `langhaxe` library I made to do it.