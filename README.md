> [!WARNING]  
> I ran this through Chatgpt to spell check for me because I am lazy. Let me know if a link doesnt work or something is wierd.

# interesting_things_of_mine

To my own dismay, I don't have much publicly facing code of that I am particularly proud of, and the private code I have is private because I am too embarrassed to show it publicly. I'll work on this.

Most of the code I've written is in a Monorepo somewhere in Star Atlas Space. The examples below don't represent my everyday work. Most of my day to day work included more boring stuff like. I have a private repo atm of some web code but I don't want to make that public, but for an idea it is a Turborepo where I am experimenting with Solidjs and some other CSS libraries. I am also using Railway.app to deploy some code, and will eventually run some kind of crank that does something idk.

A couple of things I find interesting.

### Bots

---

I love bots and have found packages like playwright and puppeteer insanely powerful. These were some of the first implementations I made a couple of years ago that log into services and perform actions. There is an entire engineering discipline to be discovered in botting and scraping. This [talk](https://www.youtube.com/watch?v=RsC4VGztDlg) is a huge inspiration and provides a bit of an idea of how creative botting can be another tool in the tradesmen's chest.

[A Tinder bot that would drop a pickup line after a match would occur.](https://github.com/caspercasanova/slave1/blob/master/tinderbot.js)

[A SoundCloud bot that I would post to Twitter if I liked a song on SoundCloud. The check would run on intervals of 15 minutes.](https://github.com/caspercasanova/slave1/blob/master/soundbrain.js)

> [!NOTE]  
> You can probably find my music selection from that script. So long as SoundCloud is free, I will use it as my main source of music, that and YouTube.

### Gaming

---

In my mind, game devs are crazy and the breadth of knowledge to make a game is crazier. Solid game devs should be paid more. After being laid off from Star Atlas, I dipped my feet into Godot and found a lot of transferable knowledge from my web dev experience. Attempting to make _something... \*\*anything really_\*\* in Godot was eye-opening.

[Durer's Solid](https://github.com/caspercasanova/Durers_Solid).

> [!NOTE]  
> Referencing Melancholia II. The solid could represent a couple of things, but I like the idea that it was Durer's attempt at creating a perfect form or a Quintessence. Durer is possibly admitting the futility, and eventual despair, in chasing perfection.

The code below shows a sequence something like this sequence.

1. NPC fires a weapon
2. Weapon shoots a bullet (potential for different bullet types exist) and attaches the NPC ID to the bullet along
3. Bullet collides with the Hitbox of the NPC.
4. NPC registers the Bullet Damage type and performs `take_damage()` method

- if the target NPC dies, the target NPC runs something like `sender.killed_target(me)`

5. Bullet collides with a wall and stands still for 1 second and explodes
6. That explosion collision box collides with the NPC collision boxes and registers a Blast Damage type.

[Damage Source](https://github.com/caspercasanova/Durers_Solid/blob/main/globals/Damage_Source.gd)

[Basic Gun Use](https://github.com/caspercasanova/Durers_Solid/blob/main/weapons/blaster_a/blaster_a.gd#L37)

[Basic Bullet](https://github.com/caspercasanova/Durers_Solid/blob/main/weapons/bullet.gd#L24)

[Basic NPC](https://github.com/caspercasanova/Durers_Solid/blob/main/npcs/dummy/dummymale.gd)

[NPC Damage Taken](https://github.com/caspercasanova/Durers_Solid/blob/main/npcs/dummy/dummymale.gd#L426)

The entire repo is chaos, and at the moment I like it like that. I will show you how to run the code on a call if you'd like.
For reference, I took A LOT of code from this repo. It's written in CPP, but I used chat GPT to help me understand what was going on. HEAVY HEAVY HEAVY influence comes from this.
[Source SDK](https://github.com/ValveSoftware/source-sdk-2013/blob/master/mp/src/game/shared/takedamageinfo.cpp#L386)

- Also, the [Damage Source File](https://github.com/caspercasanova/Durers_Solid/blob/main/globals/Damage_Source.gd) has the links to a lot of referenced code in the Source SDK

> [!NOTE]
>
> ### A note about Half-Life
>
> In watching some Half-Life retrospectives and post-mortems, I learned that the Gravity Gun in Half-Life 2 was originally a debugging tool. Eventually, the Gravity Tool became fun to use, and the devs decided to give the player the tool, and the game of the year was born. In fact, at the same time Valve was working on Half-Life's physics engine, Id Software AT THE SAME TIME had their own physics debugging tool and opted against giving it to the player for fear it would "make the player too powerful." I take that entire history as a huge lesson. Good tools can make or break a product, so I keep my eyes out and ask myself often "Can I make a tool for that?".

[I think this is the video for the Half Life Retrospective I am talking about](https://www.youtube.com/watch?v=BQLEW1c-69c)

- Go to 52:18

### Devs & Inspos

---

Here's some other things I find interesting. Will add more in time.

[JWZ](https://www.jwz.org/)

[Primagen](https://www.youtube.com/@ThePrimeagen)

[A cool code garden](https://garden.bradwoods.io/)

### Final Thoughts

---

I am more of a compiler than an inventor at this stage of my career but aim to evolve in the coming years to be a well-rounded inventor of new things.
