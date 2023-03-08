# Features Added to the Engine
This is all of the functionallity provided to the engine. The first part of this list is additions specified by Monash University, the second part of the list is additions made by the team.

## Features designed by Monash Uni:

### Trees:
_A Tree has three stages/cycles and each stage has a unique spawning ability. It takes 10 turns to grow into the next stage._

#### Sprout:
- It has a 10% chance to spawn Goomba on its position in every turn. If any actor stands on it, it cannot spawn Goomba.
It takes 10 turns to grow into a small tree/Sapling (t)

#### Sapling:
- It has a 10% chance to produce/spawn a coin ($20) on its location at every turn. 
- It takes another 10 turns to grow into a tall tree/Mature(T)

####  Mature (T):
- It has a 15% chance to spawn Koopa in every turn. If an actor stands on it, it cannot spawn Koopa.
- For every 5 turns, It can grow a new sprout (+) in one of the surrounding fertile squares, randomly. If there is no available fertile square, it will stop growing sprouts. At the moment, the only fertile ground is Dirt. (Edit: remove 'spawn' keyword in this bullet point)

-It has 20% to wither and die (becomes Dirt) in every turn

### Jumping:
_A Super Mario game will not be complete without a "jump" feature. When the actor is standing next to the high ground, the actor can jump onto it. Going up requires a jump, but going down doesn't require it (the actor can walk normally). Each jump has a certain success rate. If the jump is unsuccessful, the actor will fall and get hurt. The success rate and fall damage are determined by its destination ground as listed below_


- Wall: 80% success rate, 20 fall damage
- Tree
  - Sprout(+): 90% success rate, 10 fall damage
  - Sapling(t): 80% success rate, 20 fall damage
  - Mature(T): 70% success rate,  30 fall damage
  

### Enemies:

#### Goomba (g):
_Goombas /ˈɡuːmbə/, known in Japan as Kuribo, are a fictional mushroom-like species from Nintendo's Mario franchise. Goomba is a basic enemy. In Japan, Goombas are called "Kuribō", which loosely translates as "chestnut person"_
- It starts with 20 HP
- It attacks with a kick that deals 10 damage with 50% hit rate.
- In every turn, it has a 10% chance to be removed from the map (suicide). The main purpose is to clean up the map.

#### Koopa (K):
_Koopa Troopas, commonly shortened to Koopas or Troopas, known in Japan as Nokonoko, are reptilian mini-troopers of the Koopa Troop from the Mario franchise. When defeated, Koopas may flee from or retreat inside their shells._

- It takes 10 turns to grow into a small tree/Sapling (t)
- It starts with 100 HP
- It attacks with a punch that deals 30 damage with a 50% hit rate.




### Magical Items:

#### Super Mushroom (^):

_Anyone that consumes Super Mushroom will experience the following features. The effect will last until it receives any damage (e.g., hit by the enemy). Once the effect wears off, the display character returns to normal (lowercase), but the maximum HP stays._

- Increase max HP by 50
- The display character evolves to the uppercase letter (e.g., from m to M).
- It can jump freely with a 100% success rate and no fall damage.

#### Power Star (*):

_Power Star cannot stay in the game forever. It will fade away and be removed from the game within 10 turns (regardless it is on the ground or in the actor's inventory). Anyone that consumes a Power Star will be healed by 200 hit points and will become invincible. The invincible effect replaces fading duration (aka, fading turn's ticker stops). Here, the invincible effect lasts for 10 turns._

- Higher Grounds. The actor does not need to jump to higher level ground (can walk normally). If the actor steps on high ground, it will automatically destroy (convert) ground to Dirt. 
- Convert to coins. For every destroyed ground, it drops a Coin ($5).
- Immunity. All enemy attacks become useless (0 damage). 
- Attacking enemies. When active, a successful attack will instantly kill enemies.


### Trading:

#### Coin ($):
_The coin is the physical currency that an actor/buyer collects. A coin has an integer value (e.g., $5, $10, $20, or even $9001). Coins will spawn randomly from the Sapling (t) or from destroyed high grounds. Collecting these coins will increase the buyer's wallet (credit/money). Using this money, buyers (i.e., a player) can buy the following items from Toad_

- Wrench: $200

- Super Mushroom: $400

- Power Star: $600



#### Toad (O): 
_Toad (O) is a friendly actor, and he stands in the middle of the map (surrounded by brick Walls -- basically, put Toad somewhere near Mario at the starting point). You will have an action to speak with Toad. Toad will speak one sentence at a time randomly:

- You might need a wrench to smash Koopa's hard shells."

- You better get back to finding the Power Stars."

- The Princess is depending on you! You are our only hope."

- Being imprisoned in these walls can drive a fungus crazy :("_
    
_Once the player holds a Wrench, he won't say the first sentence. When the Power Star effect is active, the second monologue must not be printed in the console. Other than these two scenarios, he will randomly pick a monologue above._
    
### Reset Game
_Sometimes, the game can become overwhelming and it is hard to walk around (too many Koopas!). Mario has an action to reset the game at any time. If it is executed, it will do the following:_

- Trees have a 50% chance to be converted back to Dirt

- All enemies are killed.

- Reset player status (e.g., from Super Mushroom and Power Star)  

- Heal player to maximum

- Remove all coins on the ground (Super Mushrooms and Power Stars may stay).

_Mario can only do this once throughout the entire game._ 



## Features designed the Team

### Forbidden Magic:


###### RUINS:
- A structure on the original game map with high difficulty walls to jump over.
- 2 Guard Koopas patrol the doorway.
- There are 2 ways in – jump over the walls (hard) or kill the guards.
- Inside is a new item, a necromancy weapon (N).

###### NECROMANCY WEAPON:
- This weapon can bring a dead enemy back to life to fight for the player
- If the necromancy weapon is in the players inventory, the corpses of fallen enemies will remain on the map for 5 turns, during which time they can be turned into a Zombie
- Zombie will seek out and attack other enemies on the map. There is only one type of reanimated enemy (zombie). Zombies have a 'z' icon and deal 10 damage with a 50% hit rate. Zombies will not try and attack domant koopas. 
- Reanimated enemies are active for 20 turns, after which their body deteriorates, and they die forever (removed from the map).
- Weapon starts off with 10 damage and 30% hit rate. Every time something is killed with the weapon, the damage increased by 5 and the hitrate increases by 5%

### Mining:

###### SHOVEL
- This is an item that you can buy from Toad
- It allows you to dig at ‘diggable’ grounds 

###### SPORES
- Spores are a type of ground
- It can be walked on like normal dirt 
- By stepping on Spores ground, you step into the cloud of spores. For each turn that you end in the spores, you take 5 points of damage

###### SOFT GROUND
- Soft ground is a type of ground
- It can be walked on like normal dirt
- When an actor is on soft ground - and has a shovel in their inventory - they have a Dig Action available to them. 

###### DIG ACTION
- The player must have a shovel in order to be able to take the dig action while on soft ground. 
- When you dig, you have a 75% chance of digging up a $50 Coin (which sits on the ground and can be picked up), and a 25% chance of digging up a ‘clump of spores’, which immediately covers a 3*3 area centred on the place you dug, and lasts for 10 turns

