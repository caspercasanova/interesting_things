# interesting_things

To my dismay I don't have much publically facing code that I am particularly proud of and the code that is private is because I am too embarassed to show it publically.  

A couple things I find intersting. 

### Bots 
---
I love bots and have found packages like playwright and puppeteer insanely powerful. These were some of the first implementations I made a couple years ago that log into services and perform actions. There is an entire engineering disicpline to be discovered in botting and scraping. This [talk](https://www.youtube.com/watch?v=RsC4VGztDlg) is a huge inspiration and provides a bit of an idea of how creative bot netting can be another tool in the tradesmen's chest.  
 
[A tinder bot that would drop a pickup line after a match would occur. ](https://github.com/caspercasanova/slave1/blob/master/tinderbot.js)

[A soundcloud bot that I would post to twitter if I liked a song on Soundcloud. The check would run on intervals of 15 minutes. ](https://github.com/caspercasanova/slave1/blob/master/soundbrain.js)
- You can probably find my music selection from that script. So long as Soundcloud is free I will use it as my main source of music, that and youtube. 


### Gaming
--- 
Gave devs are crazy in my mind. The breadth of knowledge to make a game is crazy and game devs ought to be paid more. After being laid off from Star Atlas, I dipped my feet into Godot and found a lot of transferable knowledge from my web dev experience. Attempting make _something, anything really_ in godot was eye openning. 

Durer's Solid. - Referenecing Melacholia II. The solid could repesent a couple things, but I like the idea that it was Durer's attempt at creating a perfect form or a Quintessence. Durer is possibly admitting the futility, and eventual despair, in chasing perfection. 

The code below shows something like this sequence. 
- NPC fires weapon
- Weapon shoots a bullet (potential for different bullet types exist) and attaches the NPC ID to the bullet along
- Bullet collides with the Hitbox of the NPC.
- NPC registers the Bullet Damage type and performs `take_damage()` method
  - if target npc dies, target npc runs something like `sender.killed_target(me)`
- Bullet collides with wall and stands still for 1 second and explodes
- That explosion collision box collides with the NPC collision boxs and registers a Blast Damage type.  

[Damage Source](https://github.com/caspercasanova/Durers_Solid/blob/main/globals/Damage_Source.gd)
[Basic Gun Use](https://github.com/caspercasanova/Durers_Solid/blob/main/weapons/blaster_a/blaster_a.gd#L37)
[Basic Bullet](https://github.com/caspercasanova/Durers_Solid/blob/main/weapons/bullet.gd#L24)
[Basic NPC](https://github.com/caspercasanova/Durers_Solid/blob/main/npcs/dummy/dummymale.gd)
[NPC Damage Taken](https://github.com/caspercasanova/Durers_Solid/blob/main/npcs/dummy/dummymale.gd#L426)

The entire repo is chaos and at the moment I like it like that. 
For reference I took ALOT of code from this repo. Its written in CPP but I used chat GPT to help me understand what was going on. HEAVY HEAVY HEAVY influence comes from this. 
[Source SDK](https://github.com/ValveSoftware/source-sdk-2013/blob/master/mp/src/game/shared/takedamageinfo.cpp#L386)
- Also the damage source has the links to a lot of refernced files in the Source SDK

### A note about Half Life


In watching some Half Life retrospectives and post mortums I learned that the Gravity Gun in Half Life 2 was originally a debugging tool. Eventually the Gravity Tool became fun to use and the devs decided to give the player the tool and the game of the year was born. In fact, at the same time Valve was working on Half Life's physics engine, Id Software AT THE SAME TIME had their own physics debugging tool and opted against giving it to the player for fear it would "make the player too powerful." I take that entire history as a huge lesson. Good tools can make or break a product so I keep my eyes out and ask myself often "Can I make a tool for that?". 


### Final Thoughts. 
--- 
I am more of a compiler than an inventor at this stage of my career, but aim to evolve in coming years to be a well rounded inventor of new things.

Heres some coders I find interesting. Will add more in time.  
[JWZ](https://www.jwz.org/)
[Primagen](https://www.youtube.com/@ThePrimeagen)
