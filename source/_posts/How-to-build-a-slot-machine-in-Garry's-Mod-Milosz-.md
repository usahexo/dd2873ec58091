---
title: How to build a slot machine in Garry's Mod Milosz 
date: 2022-11-19 19:16:51
categories:
- Casino Royale
tags:
---


#  How to build a slot machine in Garry's Mod Milosz 

In this article, we will create a very simple slot machine in Garry's Mod using the Milosz Library. The Milosz Library is a library that allows you to create games in Garry's Mod.

The first step is to create a new project in the Milosz Library. To do this, open up Garry's Mod and go to Tools > Milosz Library > New Project.

The next step is to select the Slot Machine template.

Once you have created the project, you will need to import the required libraries. To do this, go to File > Project Settings and then select the Libraries tab.



You will need to import the following libraries:
- Milosz
- Lua
- Math
- Physics
- Game Instance

Now that the libraries are imported, we can start creating our slot machine. The first thing we need to do is create a new table called SlotMachine. This table will hold all of the information about our slot machine.


Here is an example of what the SlotMachine table might look like:

    "name"  : "Slot Machine" ,    "description" : "A simple slot machine." ,    "image_path" : "Images/SlotMachine.png" ,    "width" : 60 ,    "height" : 30 ,  

Now that we have created our SlotMachine table, we can start creating our slots. Each slot will have its own set of properties that we will need to define.


Here is an example of how a slot might be defined:

   "slot_name" : "Coin Slot" , 							 "slot_image" : "Images/CoinSlot.png" ,                  // The image file for the slot machine image.                  "type" : "coin_slot" , // The type of slot machine. Must be one of 'coin_slot', 'card_slot' or 'cash_slot'.                                   // Additional properties specific to this type of slot machine.                  },

#  How to make a roulette wheel in Garry's Mod Milosz 

In this tutorial, you will learn how to create a working roulette wheel in Garry's Mod. First, you will need to create a model of a roulette wheel. You can do this by using a modeling program such as Blender or Cinema 4D. Alternatively, you can find a 3D model online and import it into Garry's Mod.

Once you have created the roulette wheel model, you will need to create a prop_dynamic entity for it. In the entity properties, set the "Gravity Scale" to 0 and the "Mass" to 0. Next, add the following lines of code to the "models" section of the entity:

"wheel": { "file": "<path-to-wheel-model>", "scale": <wheel-scale>, "rotation_x": <angle-for-x-axis>, "rotation_y": <angle-for-y-axis> }

The "wheel" property defines the name of the model that will be used for the roulette wheel. The "file" property defines the path to the wheel model file. The "scale" property sets the scale of the wheel model. The "rotation_x" and "rotation_y" properties define the angles for the x and y axes respectively.

Finally, add these lines of code to enable physics on the wheel:

"Physics": { "Enabled": true },

The "Physics" section defines whether physics should be enabled on the wheel. Set this to true if you want the wheel to be interactable.

#  How to make a dice game in Garry's Mod Milosz 

In this article, you will learn how to make a dice game in Garry's Mod. First, we will create the basic game structure, then we will add the functionality to roll the die and move our player character.

To get started, create a new file in your favorite text editor and save it as "dicegame.lua". Next, we will create a table to store the game state:

local gamestate = { }

Next, we will write a function to initialize the game state:

local function init ( ) 
 local player = UTIL . Spawn ( "player" ) 
 gamestate . player = player 
end

This function will spawn a player character and store it in the gamestate table. Now let's add some code to handle the die roll:

local function roll ( ) 
 return math.random ( 1 , 6 ) end

This function will generate a random number between 1 and 6. We can use this function inside our init function to start the game:


init ( ) 

Now that our game is initialized, let's add some code to move our player character:

function update ( dt ) 

 if gamestate . player . dying then return end 
gamestate . player : MoveVector3D ( roll ( ) * 50 , 0 , 0 ) 
end

In this function, we first check if the player is dying. If they are, we exit the function. Otherwise, we use the roll() function to generate a random number and multiply it by 50. This will give us a value between 0 and 250 which we can use to move the player character. Finally, we update the gamestate table with the new values. Now let's run our game! To do this, open up Garry's Mod and navigate to "Tools > Scripts > Run Script". Then select "dicegame.lua" from the list of files. You should see something similar to this:





The game is displayed in spectator mode as it currently has no players. Let's fix that! First, click on "Tools > Addons > Hammer Editor". This will open up Valve's Hammer Editor which is used to create levels for Garry's Mod. Next, click on "File > New". A new window should appear with several options - select "Map" from the list and click "OK". This will create a new level for our game. Now let's add some props so that our player can interact with them. Navigate to "Architecture > Prop Gallery" and select "de_dust2". This prop set includes several objects that we can use in our game. Drag-and-drop one of these props onto your level - I've selected "func_door_rotating". Now let's configure it so that it behaves like a die. In the Properties panel on the right-hand side of the screen, find the "Solidity" field and set it to "None". This tells Garry's Mod that our prop is not solid and can be passed through by players. Next, find the "Touch activated?" field and set it to "Yes". This tells Garry's Mod that players can interact with our prop by touching it. Finally, find the "Targetname" field and set it to "die1". This gives our prop a name which we can use later in our code. Now let's add another prop so that players can see their score: navigate back to Prop Gallery and select "textLabel". Drag-and-drop this onto your level and configure it as follows:  Name: Score  Text: Your Score is: %s  Font Type: Comic Sans MS Bold 24pt Now let's add some code so that players can interact with these props. In your script file, add the following functions: local function onStart ( ply )  die1 : Kill ( ply ) end local function onScoreUpdate ( ply , score ) textLabel : SetText ( score .. "%s" ) end These functions will handle events that occur when players start or update their score respectively. We first kill off our die1 prop so that it respawns with each turn. We then update our textLabel prop with the current score value for players to see. Finally, we need to connect these functions to our props using Input Handlers - Click on die1 in Hammer Editor and then find the button labelled "<>" in the bottom-left corner of its Properties panel). Click this button and select onStart from the list of functions that appears.:

Now let's test out our game! Press F9 while playing your level in Hammer Editor mode to enter debug mode - this allows you to run your game without having to load it into Garry's Mod first. You should now see something similar to this:





Press E on your keyboard or left-click

#  How to make a poker table in Garry's Mod Milosz 

In this article, we are going to make a poker table in Garry's Mod. 

First, we need some materials. For the base of the table, we will need six wooden boards that are each eight feet long and two inches wide. We will also need a piece of plywood that is four feet by eight feet. For the sides and top of the table, we will need six pieces of wood that are each two feet long and two inches wide. Finally, we will need some screws, a drill, a saw, and sandpaper. 

Once we have gathered all of our materials, we can begin constructing the table. The first step is to cut the boards for the base of the table. We will want to cut two boards that are each four feet long and two boards that are each two feet long. We can then assemble the base of the table by screwing the four boards together. 

Next, we will want to cut the plywood sheet into eight equal pieces. We can then screw these pieces onto the top of the base that we just created. 

Now it is time to create the sides and top of the table. We will want to cut six pieces of wood that are each two feet long and two inches wide. We can then assemble these pieces into a rectangular frame by screwing them together. We can then attach this frame to the top of the table with screws. 

Finally, we can sand down any rough edges with sandpaper until our poker table is smooth to the touch. And that's it! Our poker table is now complete!

#  How to make a blackjack table in Garry's Mod Milosz

In Garry's Mod, there are many things you can create with the physics engine and Lua scripting. One of the most popular games you can make is a blackjack table. This guide will show you how to make one.

1) Creating the Table

The first step is creating the table. This is done by creating a cube and resizing it to be the size of a table. You can then use the "func_illusionary" entity to create a flat surface on top of the cube. This will be our table.

2) Creating the Cards

Next, we need to create the cards. This is done by creating rectangles and using the "prop_dynamic" entity to create an image on them. We then give them a random rotation and set their health to 0 so they can't be picked up.

3) Creating the Deck

The deck is created by creating a large number of cards and setting their parent to "deck". We also give them a random rotation and set their health to 0 so they can't be picked up.

4) Spawning the Players

Now that our game is ready, we need to spawn players at the table. We do this by creating an "env_player_team" entity and setting its targetname to "player1" (or whatever you want your player's name to be). We also give it a team number of 1 (red team). We then do the same thing for player 2, but set its team number to 2 (blue team).