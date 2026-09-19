# Once Upon

Terrain gen mods are some of the most impressive mods in minecraft not just in terms of creativity, but also the painstaking detail put into making them look absolutely perfect.

However, most of them are incredibly pretty, but lack the element of playability and weirdness that makes vanilla Minecraft's terrain oftentimes better for the average playstyle. Which sucks because vanilla terrain tends to be boring and nowhere near as stunning to look at as mods like Tectonic or Big globe.

Most of these major terrain gen mods also don't generate terrain that's meant to be enjoyed at a smaller scale. Most of the joy of these terrain gen mods comes from what you can see out in the distance, rather than what's right in front of you. 

And for a very large majority of players, that's how they want their world. Advancements in LOD and shader technology have made this kind of playstyle (Where the terrain's main focus is faraway rather than near) much more aesthetically pleasing and accessible than it ever has been. 

However, there's still quite a decent chunk of players (Ironically mostly veterans who remember early terrain) who want their terrain to be jagged and weird rather than distant and epic. 

I should also state that this mod does add epicness and verticallity to the world, but it's implementation of that adds it more through big cliffs, weird spires, as well as a healthy sprinkling of jagged looking mountains rather than big sweeping features as seen in tectonic.

# How does it work? 

Once Upon is entirely data based. Originally I had developed a whole system that involved a tectonic plates simulation (That I'm still a little sad went unused), but that whole system was too hard to integrate with minecraft's existing system, mainly because minecraft uses a 3d density function, and my simulation just took a heightmap and replaced the density function with an interpolated heightmap checker.

Due to the hydrology simulation (which would have cost me my sanity to write deterministically) requiring the whole map heightmap upfront to run, trying to generate a full world at full resolution at a reasonable size (10k by 10k) with mutliple channels would have been a little RAM heavier than I would have liked (roughly 400MB with all the needed channels and masks), and would have made world load in extremely long. Possibly mutliple hours.

Using a heightmap also didn't produce nice results, they looked too rounded, and rather than produce messy overhangs like a datapack did, it made steep but rounded edges which I thought looked sub par for what I was aiming for. 

TLDR; Data only, we tried a full geology sim but it looked awful

# Why is it so minimal? 

This mod is a side - side project of mine, I'm the dev of Ecstatic, and this project is a fun little experiment. Currently structures are being worked on, maybe some biome tweaks, tons of fun stuff being planned. Right now it's the terrain gen datapack in its rawest form.
