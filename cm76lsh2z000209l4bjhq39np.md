---
title: "SAP Devlog: 2/15/2025"
datePublished: Sat Feb 15 2025 19:41:23 GMT+0000 (Coordinated Universal Time)
cuid: cm76lsh2z000209l4bjhq39np
slug: sap-devlog-2152025
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1739640009863/73604d5e-a5d1-45ff-9080-c90a37ee7ef2.png
tags: devlog, sinco

---

Would you like to help on Sinco and Portilizen? Fill out this google form: [https://forms.gle/YG4KV71dWmuPRZaA8](https://forms.gle/YG4KV71dWmuPRZaA8).

When it comes to the Pre-Alpha stage of the game I am hoping to give a fun little demo for people to play.

The day before valentine’s day (2/13/2025) I had created an “INDEV ROADMAP” and It starts with the Prototype in February, moving to the Pre-Alpha from February to March. But at the rate I’m going I think the Pre-Alpha might come sooner.

If I had to give a rough estimate I think near the end of February is most likely.

But onto actual work.

# 2/14/2025: Post-devlog

## 0.0.4-p development

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

Anyway, after fixing some more screenshot bugs and fixing a world map bug I released 0.0.4-p in the development span of 1 day. It took 0.0.1-p 3 days, 0.0.2-p 4 days, 0.0.3-p 7 days, and 0.0.4-p 1 day. The development time went up and up, and then went WAY down. And the cause? Motivation! My motivation to work on the game has gone WAY up! And it shows, I’m making a 5+ minute read blog post about development! While developing!

## 0.0.5-p development

Anyway continuing on I worked on an Osin Attack Indicator and now I feel like the stage is too easy but I can work on difficulty stuff later.

I want there to be a more customized sound tray, so I started working on it in a separate branch but I can’t figure out how to add FlxSprites, and I don’t know how Bitmaps work… so uh. Let’s see what FNF does with it. And now that I know, I worked with it, added some offsets to things so everything fits and boom.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739586186507/f98cf118-38a0-421c-8f2e-e3463042b7fa.png align="left")

A more cool sound tray.

Anyway, what next? Let’s check the TODO.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739589507743/a480cc2b-0404-4038-a06b-5b54f367ad33.png align="left")

Ugh. Ok, let’s do Localization. `hmm install langhaxe`, add save stuff for language. Now for the langhx file. After going through all the states where I could use `PhraseManager.getPhrase()` and after a bit these are all the phrases I had to make:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739591779409/5cc37519-df0c-4247-8c2b-b69ec5b0d938.png align="left")

remember when I said “The amount of text in the game at the time had scared me out of it.”? Yeah no I really under-estimated how many phrases are not connected to files. Anyway I made a google-translated Spanish langhx file, Djotta Flow made a Portuguese translation, I made some build flags and fixed capital phrase keys. Made the PR and merged. Now localization is in the game via Build flags, but nah, let’s have it controlled by a text file! Make localized assets for the character ring and then I worked on it and got it working! How about .bat files that compiles localized builds for me?

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739597817335/61e8f4d3-a555-407f-8b92-94a8750dacb7.png align="left")

Done! Why is this Localization thing so fun lmao!

Y’know I wanted to do a loading screen not too while ago but then I asked myself: what would I be loading? So yeah that went down the road.

I just thought about how Haxeflixel manages plugins and I’m thinking about doing that for mods, source code mods anyway.

# 2/15/2025: 12AM - 1AM

And after like 200% of my sanity being set to null I got something that works.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739602562560/97284ffd-f61c-47e8-8989-a8bd33e67941.png align="left")

Dynamic functions is the result of my suffering, but I can’t stop now. Sadly. I get some things set as public static vars and went to bed

# 2/15/2025: Post-sleep

After a nice good nights sleep my sanity is once again a thing.

I started working on events, basically a bunch of signals being called. I have this piece of code:

```plaintext
override function onStateSwitchComplete() {
                super.onStateSwitchComplete();

                if (FlxG.state == new TitleState())
                {
                        trace('Title!');
                }
        }
```

which doesn’t give an error. It just doesn’t work. I put out a help me message on the haxe discord

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739628453943/758d6dee-1f85-49c5-927e-acf96133c714.png align="left")

and now I'm gonna work on other things.

Oh,

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739628571506/4ae35da1-b13e-4290-9b4d-9efa34b19e39.png align="left")

ain’t that nice? And it works too!

Now what the hell is this?

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739628633497/c4130b20-e6cc-4313-9628-5bd904444b98.png align="left")

Uhm. Anyway, fixing that several times cause you can’t initialize custom `FlxState` classes that loads graphics in public static vars apparently, anyway, I’m modding basically every state I can get my hands on in whatever way. Lol.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739631267909/7f7a9d59-9697-4f58-8883-7e2e06a69cdd.png align="left")

Let’s mod the Stages shall we?

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739632444113/d2b22964-8397-4ef3-9c51-21f878b29222.png align="left")

In theory with this mod system I could modify the world map to have more levels and to have levels unlocked, so the stages technically could already be modular. The only issue I think MAYBE, would be editing it with other mods but with dynamic functions there is none so lol, I dumb sometimes lmao.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739633192901/da2cd208-1f7e-4bcf-89f4-e0cbe9a416d2.png align="left")

These little modifications for these sections of the game are fun to make once everything works.

Key phrase: once everything works. Cause OH, MY, FUCKING GOD.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739634586185/dc6bc8fb-831c-4284-8645-4d839ee560e8.png align="left")

I’ve gotten more errors like this than ever. And the issue for that one was ONE line of code getting modified.

Also then the press any sprite stopped getting properly visible? It looked like the tween wasn’t working for some reason so I had to debug that.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739635463557/3b08b965-31f7-4f75-9cf1-38f6cfb40cbc.png align="left")

Alright, I fixed that in a dumb way but it’s fine. Now let’s get-

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739636152644/3ce6ac0e-505b-4209-b60c-0d2cc2b97a00.png align="left")

🥲

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739636190194/b7ca67e0-9591-4d71-b5b9-74ed40020727.png align="left")

Uhm. What?

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739636246444/49f434fe-cd06-4e62-90b8-00376ed43f28.png align="left")

Alright. Fixed it. And now my inputs don’t work, great.

Another one line fix and we should be good, right?

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739636338144/3424fc52-d8b1-4b32-ae75-483fa8103fb1.png align="left")

Never.

I’m noticing a pattern of these being because of the public static variable classes getting initialized outside a function.

Anyway. After 20 years, I finally stopped getting crashes, and could merge into main.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739637308827/013c5169-e9be-47bb-9079-3d32dfec5b76.png align="left")

Feels so fucking good.

Anyway I’m taking a break from coding for a bit and I’m focusing on localization assets. Same with DJ, he is doing the Portuguese “Press any to play” asset while I do the Spanish. I finished and I liked it to a certain degree, some of the letters looked wrong but it’s fine, DJ finished the Portuguese asset and I realized I forgot the exclamation mark, whoops, turns out it changes most of the words though so I’m gonna just delay redoing the asset.

I separated the Character ring Characters from the ring and coded that up and it looked the same, which is good so yeah.

Anyway back to the Spanish asset. I quickly did it, and it looks nice.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739639122601/7fef30a4-a904-4cba-8134-aed4b103131b.png align="left")

So now I’m checking how the assets look in game and yeah, they look good.

Spanish:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739639195669/611cd04b-5a19-4b9f-9da1-305a9fd47c64.png align="left")

Portuguese:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739639316926/f49e1993-bcb5-4077-924c-a5214c2a8223.png align="left")

I feel flexed on with the Portuguese one because he fixed the R in the “press any to play” text.

But anyway, I still didn’t wanna do much coding so I made the cover for this devlog! I like it alot, it’s not like the OST thumbnail but it’s something.

Still don’t wanna do coding and I just wrote about OST? Lets make result theme tracks! There are 6 ranks so I will make 6 tracks. Or will I? If I make 4, Awful and Bad can share one song, good and great can share one, and excellent and perfect have their own tracks separate from each other! I say that’s a plan! And yeah I did it, they are very nice to listen to, had to change up some systems and add a new Global function but other then that the process on making and adding the music to the game was peachy. I also made the Results State a bit more moddable since well, why not?

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739644904200/1550c017-7df4-4b5c-bc35-832e9432c5f4.png align="left")

I get that and I like that. I’ll work on making it more more moddable another time.

Time for a break!

Chicken nuggies.

Anyway after that I don’t actually know what to work on lol. So Imma call 0.0.5-p finished, and release this devlog.

See you next time!

Look at all these terminals though.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1739647347843/bdf09677-e3d6-4a54-bd01-a3a7784d3e76.png align="center")