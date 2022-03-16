---
title: 'My Pico-8 Adventure'
media_order: 'game-hat.png,PICO-8_logo.png,my-pico-8-game-min.jpg'
header_image: PICO-8_logo.png
date: 02-03-2022
tags:
    - Tech
    - Innovation
    - GameDev
description: 'Getting ambitious with an innovation day playing with Pico-8 and a Raspberry Pi + Game HAT'
cover_image: ''
published: true
---

So I've recently fallen HARD for [Pico-8](https://www.lexaloffle.com/pico-8.php). If you've not heard of it it's an indie game platform designed to make developing a game simple. It's $15 and runs on a host of machines ... one of which being a Raspberry Pi!

With my new found love of small indie games, my passion for tech, a spare Raspberry Pi 4B lying around (I got when I joined the Raspberry Pi Foundation ... THANK YOU!) and an innovation day fast approaching I came up with a plan:
1. I want to build something both physical and virtual.
2. I want to utilise my new Pi.
3. I want my young boys to love my creation.
with step 3 being the real test and determines if I succeeded or not.

A few days before the innovation day I did some googling and found this beast, a [Game HAT for Raspberry Pi](https://www.waveshare.com/game-hat.htm).

![raspberry-pi-game-hat](/media/game-hat.png)

Perfect. I'd heard of but never used RetroPie, now seemed like the perfect opportunity. There were tons of blogs, articles and comments about getting Pico-8 working on a RetroPie machine, my favourite being this [reddit post](https://www.reddit.com/r/RetroPie/comments/lurmu0/pico8_in_retropie_easy_uptodate_tutorial_with/), nice easy-to-follow steps with working links to code snippets, thanks rhinofinger!

That's the physical done - check. I'm also utilising my new Pi - check. Happy days.

Next onto Pico-8 game developing. I've tinkered with PyGame in the past and just want to make something simple and repetitive, my boys will love it. I'd previously made 80% of a game with my eldest which was a simple platformer with obstacles to avoid. Nothing too adventurous and plenty of room for expansion. So my plan is to:
- make a single character
- make a single background
- add platforms to the level
- add obstacles moving from one side to the other

This could be expanded in each area with:
- a character selection
- moving background and/or multiple locations
- randomise platform locations and/or increase/decrease number of platforms for different difficulties
- change obstacle size, location, speed

Lovely, looks like a decent plan!

### ... some time later ...

That was an AWESOME DAY!!! Pico-8 ... love it, game HAT ... love it, RetroPIE ... LOVE ... IT! Lua ... I might learn to love it.

I feel I was a little ambitious for the day. I've got my build, Pico-8 works with SPLORE (although I need to do a hard reboot to exit). My very own Pico-8 game is still very much based off tutorials. I've got a little man that can move left and right on something that looks like grass but other than that he can't do much.

![my-pico-8-game](/media/my-pico-8-game.png?resize=400,200)

Still my boys were pretty chuffed so I'm counting all of this as a massive win and something else to do between things.

#### Useful Links

- [A simple pico-8 game tutorial](https://tongullman.blogspot.com/2016/10/pico-8-introductory-tutorial.html)
- [Pico-8 wiki ... a fountain of knowledge](https://pico-8.fandom.com/wiki/Wiki)
- [An awesome example of a platformer for $1](https://2darray.itch.io/tinyplatformer)
- [A good ol' fashioned cheatsheet](https://eugene.libguides.com/ld.php?content_id=42775909)