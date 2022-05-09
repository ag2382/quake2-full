# Quake II: Zelda Edition <img src = "https://user-images.githubusercontent.com/90282143/167364436-3e780748-23f5-4cfd-8366-f37a4bd7df4d.png" width="25" height="25">

This mod changes Quake II to make it play more like a game from Nintendo's iconic "The Legend of Zelda" series. Elements and mechanics from both the 2D games and 3D games have been implemented to add to the experience.

## Common Deliverables
* Desktop shortcut to launch mod
* Separate folder containing files needed for mod to work
* README file that explains mod in detail and shows how to test deliverables
* In-game help screen to explain mod changes
* UI updates reflecting project deliverables

## Project Deliverables
* Replace Quake II weapons with Zelda Weapons
* Upgradable weapons
* 5 spells to cast
* Implement shop, with rupees as main source of currency
* 3 types of functional armor

## Zelda Weapons
The blaster has been replaced by the master sword. Each time you shoot the blaster, the bolt acts as a "sword beam". This is one of Link's recurring sword skills in the Zelda series. The bolt now disappears after travelling a set distance from the player, given that it does not hit any surface or entity. [WIP]

## Weapon Upgrades

Not fully implemented yet :(

## 5 Spells to cast

Players can choose from 5 different spells to activate during a playthrough, each with its own specified cost. Four of these spells have a set duration for 15 seconds: <br />
* FIRE
* JUMP
* SHIELD
* SPELL 

All spells include custom UI elements that are fully functional in-game. The spell system is derived from "Zelda II: The Adventure of Link". To see how this system works in more detail, open the console by pressing tilde (~) and type 'spell'. You should see the following:

![image](https://user-images.githubusercontent.com/90282143/167352895-158aae8b-4fd3-42d3-b364-92eb1a03d1c4.png)

The player starts off with 64 magic points, the default amount that Link has in the beginning of Zelda II. Each spell will be occupied with a description, followed by in-game screenshots to showcase their functionality.

## FIRE <img src = "https://user-images.githubusercontent.com/90282143/167357467-9837de00-9236-4491-b7a4-3ea8f9c37bd0.png" width="35" height="35"> <br />
The 'fire' spell allows the player to shoot fireballs out of the sword from a distance. In the context of Quake II, the particles shot from the BFG are used to portray Link's fireballs.

Default:<br />
<img src = "https://user-images.githubusercontent.com/90282143/167360164-6cc71425-d005-4341-a7ff-62a8da815dea.png" width="500" height="375"> <br />

Spell Activation:<br />
<img src = "https://user-images.githubusercontent.com/90282143/167361308-b66890bb-122b-4f9f-818e-25804388c890.png" width=500 height="375"> <br />


## JUMP <img src = "https://user-images.githubusercontent.com/90282143/167358229-70b3dd42-8935-44a3-bae2-0c60232a0505.png" width="35" height="35"> <br />
The 'jump' spell makes the player jump twice as high as before. It also increases the width span of the player's jumps, meaning that jumps will cover more horizontal distance.

Default:<br />
<img src = "https://user-images.githubusercontent.com/90282143/167365796-04cd3121-721b-4533-aea1-76b7c1a231fe.png" width="500" height="375"> <br />

Spell Activation:<br />
<img src = "https://user-images.githubusercontent.com/90282143/167365826-830be937-07a9-4a83-9c78-9737c482246a.png" width="500" height="375"> <br />


## LIFE <img src = "https://user-images.githubusercontent.com/90282143/167358369-dd026533-2177-4f59-884f-6d635e127be5.png" width="35" height="35"> <br />
The 'life' spell recovers some of the player's health (by 50 to be exact). It has the highest magic cost out of all the spells. 

Health recoveries will not exceed the maximum health value defined by the game, which is 100. For example, imagine a scenario where the player wants to use this spell at 70 health points. Since the player's maximum health cannot exceed 100, the amount of health the player gets back after using the spell can be obtained with this formula:

heal_amount = max_health - curr_health <br />
100 - 70 = 30

Therefore, the player will only restore 30 health points instead of 50.
  
  
## SHIELD <img src = "https://user-images.githubusercontent.com/90282143/167358395-8bf3579b-dd50-4961-b0de-4fb9beafe7a0.png" width="35" height="35"> <br />
The 'shield' spell is an ability that increases the player's defensive abilities. It reduces the damage the player takes by half. Enemy fire, self-damage from inventory weapons, fall height, etc.

Example scenario: player holds grenade in their hand

Default:<br />
<img src = "https://user-images.githubusercontent.com/90282143/167369585-dae209d3-0e53-4669-a5f9-b8f4458876fd.png" width="500" height="375"> <br />
Here, the player takes 58 damage.

Spell Activation:<br />
<img src = "https://user-images.githubusercontent.com/90282143/167369673-de89cf53-080e-4292-ae20-316884df5961.png" width="500" height="375"> <br />
Here, the player takes 29 damage.<br />

## SPELL (WIP) <img src = "https://user-images.githubusercontent.com/90282143/167358419-2c934e31-40ce-47c1-b820-f4484006d0b4.png" width="35" height="35"> <br />

  The 'spell' spell allows the player to turn several enemies into much weaker ones. It has not been fully implemented yet.

## Shop + Rupees  <img src = "https://user-images.githubusercontent.com/90282143/167375390-3a15d353-fa5b-404f-997e-49a61d67772a.png" width="23" height="30"> <br />

Enemies drop rupees on death. Armor shards are used as placeholders for rupees. Each armor shard is worth one rupee.

<img src = "https://user-images.githubusercontent.com/90282143/167371988-cf50cb87-c215-4d89-997f-cdbb3a14d0aa.png" width="500" height="375"> <br />
<img src = "https://user-images.githubusercontent.com/90282143/167372022-d56a803f-89f3-4ae2-b9e8-663b25273c77.png" width="500" height="375"> <br />

The shop has not been fully implemented yet.

## 3 types of functional armor

Only one armor has been worked on, although not fully implemented yet
* Zora Tunic ~ allows player to breathe underwater

## Other Changes
* Player marine voice lines replaced with Link voice lines ripped from these games:
  * The Legend of Zelda: Ocarina of Time
  * Super Smash Bros. Melee
* Custom sound effects for rupee collecting and spell activation
* Spells include UI elements that are fully functional in-game
* Easy mode damage scaling has been removed
