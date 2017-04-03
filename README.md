# comp130-journal
# What goes into an AAA Game (Valve).
## Introduction
I am interested what goes into a AAA game and for my reasearch journal I am going to be using Valve publications as my reasearch materials
For my own projects I can already see these little branches of code happening in certain areas like AI, Animation, Controller etc. So I am very interested in finding out what a fully formed branch of all of these systems might entail and how much detail do Valve specifically add to these systems.
## AI
There are Four stages of Artificial Inteligence the paper talks about AI Behaviour, Friendly AI, Procedural generation and Provide Game Pacing. All of these build onto each other creating a more "Robust" game. Starting With AI Behaviour this might be the first thing some one adds when creating AI a computer that will draw a straight path turn then walk etc. I see this particular problem in a lot of the student game that were created this year, mobs that walk straight paths and just follow players, and it feels very unnatural. And this is where the seperation between AAA and indie begins most people don't even think about it, but making a computer walk a path that just makes sense for people when done right won't be noticed, only when you put two examples side by side. But it goes even further than just improving the pathing, they also saved memory usage by implementing a more efficient pathing that doesn't draw the entire path possible just short "look ahead" paths. Then If you are going to have AI you might think about adding Friendly AI, now in an indie game you would most likely just get the friendly to aim at the closes enemy and shoot. But in a AAA game you have to think about game design, and fair ness, the friendly character should feel like a player. Then going up the next step you have to add interesting enemy locations Valve achieve this by giving spawn rules to all of the different enemy types things like this enemy spawns behind the player more frequently etc. And going the ultimate next step Valve also added Game pacing to the enemy spawns and frequency. 

I can see myself trying to implement more realistic path finding in my own projects, that at the very least are not straight paths. Going up the steps you can make some compromises in an indie/small team type game that might not have Friendly AI that is that complex, or levels that are long enought to require complex game pacing rules.

# Rendering Wounds

This might be a more design focused article but it is really important for a programmer to understand how much work goes into modeling the characters and now when you need to show damage dealt to the enemies you can't just create thousands upon thousands of variations of wounds for a single character, when in left 4 dead 2 the simplest infected has 24000 model variations. Valve achieved this by seperating wound meshes and then culling the damaged area of the model and attaching the wound mesh. This saved memory space and allowed to have any of the models to have up to 54 unique wounds. This is a really learnable scenario of how a programmer should be there to help the designers of how to design a certain element of the game and it requires very tigth cooperation between the programmer and designer to save time and improve the game from a indie project to a AAA quality game.

# Art Direction to Gameplay

This is one of the effects that really seperate the small indie games from AAA studios, attention to detail of how a character should look from concept art to how it should be lit in game, and what camera effects should be used to add to the atmosphere of the game. Things like head lights to a car being visible, you would not think about it in-game but that adds to the horror theme of left 4 dead. Adding grain and colour correction to the camera to help the horror theme. Looking at examples from culture like paintings and ads used in the old times to draw your characters in game realisticaly, so they fit inside your game and dont stand out but actually look part of the scene. That is going the extra mile. Now this might be more useful for a designer, but I feel like it is important for a programmer to know the ins and out of every aspect of the game, and programming lighting, shadows and everything else to make the game feel more realistic is very important, and when done right just adds to the player immersion.

# Replayable Cooperative Game Design: Left 4 Dead

This Paper expands on What AI was about, but I would like to focus on all of the actions the individual characters can draw from just to imagine the scope of the AI controller tree. With Left 4 Dead Valve tried to give players the experience of being in an zombie apocalypse and to achieve that they added a lot of unique experiences that the multiple enemies can do, it gives the enemies a sense of character. The player can recognize certain patterns and get better at the game. There are rules attached to the player things like how many times you can be revived, even things like if you are not with your team you will be punished. And how the entire AI system is made to encourage cooperation and working together. Teaching the player through failure. 

When working on small projects you dont really think about this, it is better to approach your AI as character with certain traits things like this enemy will wait for the best opportunity to attack, or this one will just charge the weakest player. 

# Water Flow
This paper talks about what goes into creating realistic water if Portal and Left 4 dead and using water flow to guide the player where to go. Water flowing around a character or object is a tiny thing you think would be unnoticable, but to my surprise playtesters took 17% less turns and traversed the level faster. Now this is the only paper that talks about something an indie game developer would not spend his time implementing things, like flow vectors, and offseting textures based on those vectors. And this is what I truly wanted to find out with this reasearch journal small pieces of work within AAA games that normally go unnoticed but some programmers and designers had a lot of work allocated to achieve this. And that what at AAA game is it takes the extra step, and tries to do something that hasn't been done before.

# Improved Alpha-Tested Magnification for Vector Textures and Special Effects
This paper talks about the effeciency of vector textures in 3D space and how Valve achieved smooth vector textures and even drop shadows, with sharp corners. Sharpnes is something that comes into play when you really have a keen eye, the average player might not notice but to a vigilant spectator it will just pop out. This again ties into with all of the previous papers and just enforces the theme that Valves main goals in their games are to have as least immersion breaks as possible. When you look at a sign withing a game you want to be able to read it but you also want to believe that that sign is withing that scene, it does not seem out of place it blends in perfectly. By doing this with vectors you avoid pixelation but now you encounter anti-aliasing which is when something looks too sharp to the point when you move the camera it really stands out. What Valve does is esentially normalise the vector texture and add it to the scene.

# Conclusion

The main difference between AAA games and Indie games is the attention to game details AAA games will spend, things like immersing the player inside your game, making him feel like he is part of this universe they built. There is a lot to learn from these papers, even the complex ones, because you do not have to implement the hardest algorithms, you can achieve some of these effects by just doing it in small amounts, and just adding a few of these will go a far way, and make your game really stand out, from the masses of indie games.

The AI Systems of Left 4 Dead
http://www.valvesoftware.com/publications/2009/ai_systems_of_l4d_mike_booth.pdf

Rendering Wounds
http://www.valvesoftware.com/publications/2010/gdc2010_vlachos_l4d2wounds.pdf

How Valve Connects Art Direction to Gameplay
http://www.valvesoftware.com/publications/2008/GameFest08_ArtInSource.pdf

Replayable Cooperative Game Design: Left 4 Dead
http://www.valvesoftware.com/publications/2009/GDC2009_ReplayableCooperativeGameDesign_Left4Dead.pdf

Water Flow
http://www.valvesoftware.com/publications/2010/siggraph2010_vlachos_waterflow.pdf

Improved Alpha-Tested Magnification for Vector Textures and Special Effects
http://www.valvesoftware.com/publications/2007/SIGGRAPH2007_AlphaTestedMagnification.pdf
