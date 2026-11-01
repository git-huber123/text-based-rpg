This is my text-based RPG, and I'm shipping it in the Hack Club program SAVEPOINT.
Playable link > https://git-huber123.github.io/text-based-rpg/index.html (this is the github page)

I had built this before in Python, but I got burnt out, used too much AI (so I didn't understand it), and it was just all over my head.
However, this time around it's pretty simple - right at my skill level.

Features:
Walk around, and explore the places.
Each location has an enemy, which does a certain amount of damage with a certain amount of health. If you win, you get a reward.
If you walk over grass, you have a chance of being ambushed. Grass is automatically converted into a path for the cost of 1 food.
Paths are safe to walk over, as they've been converted from grass.
Moving costs 1 water, but not necessarily a food since walking on paths doesn't cost food, neither does going onto a building/feature.
You can heal using food, but if you run out of food you won't be able to convert paths, which is dangerous.
Fog-of-war effect: you can only see the tiles that you've discovered, instead of seeing the whole map. Radius is 3.
|=> Tiles become discovered once you're close enough, but if you die before returning to the base, all of the cells you discovered on that "run" are gone.
\\=> If you return to the base after discovering new cells, they'll become "permanent cells", which stay even after you die.

Work-in-progress:
Upgrades at the base: you'd be able to use an upgrade tree, doing things like upgrading your storage capacity, crafting weapons (which would dissapear on death), and other things.
\\=> Note that the upgrades to your stats wouldn't disappear.

To-do/planned:
Some sort of farming system: make it so that you can't instantly get food back when you respawn, maybe you have to wait a little bit, or use fertilizer that you gather from other places.
Storage system: add a way to take important items and put them at the base, so if you die they're still at the base
Anti-soft-lock system: every now and then, convert some path tiles back into grass tiles, and add a trading system to the base, so even if you have really bad rng you can walk around a bunch, take new grass tiles, and trade them in to get better materials.
\\=> This would also involve a trading system, in which you can make fairly unfair deals, but it would prevent softlocks
Saving: Save the game to localstorage and allow the player to wipe the save as well.
