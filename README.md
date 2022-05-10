# Quake II: Zelda Edition <img src = "https://user-images.githubusercontent.com/90282143/167381733-e021ae93-5ec8-46b0-aa08-e86acec8900b.png" width="30" height="30">

This mod changes Quake II to make it play more like a game from Nintendo's iconic "The Legend of Zelda" series. Elements and mechanics from both the 2D games and 3D games have been implemented to add to the experience.

## Common Deliverables
* Shortcut that Auto-Launches your Mod
* Mod in a Separate Folder
* README file in GIT that explains HOWTO install and play / test your mod
* UI updates reflecting Personal Deliverables
* Help Screen to detail how to play your mod in game

## Project Deliverables
* Replace Quake II weapons with Zelda Weapons
* Upgradable weapons
* 5 spells to cast
* Implement shop, with rupees as main source of currency
* 3 types of functional armor

## HOW TO INSTALL
1. Create a folder in the directory containing Quake 2. Rename your folder to "q2zelda".
2. Copy all the contents from the "Link" folder into the "q2zelda" folder.
3. Create a new shortcut of quake2.exe. Send the shortcut to your desktop.
4. Right click on the shortcut and go to "Properties". Look for the target field and enter " +set game q2zelda" at the end of the line.
5. **OPTIONAL** ~ change the icon of the shortcut using the provided file: "triforce.ico"

## Zelda Weapons

* Blaster --> Master Sword (WIP)
    * Each time you shoot the blaster, the bolt acts as a "sword beam". This is one of Link's recurring sword skills in the Zelda series. The bolt now 
disappears after travelling a set distance from the player, given that it does not hit any surface or entity. <br />

* Railgun --> Magical Rod
   * This is used for Link's 'SPELL' spell.

* Other essential Zelda weapons like the boomerang, bow and arrow, and hookshot have not been fully implemented

## Weapon Upgrades

Not fully implemented yet :(

## 5 Spells to cast

Players can choose from 5 different spells to activate during a playthrough, each with its own specified cost. Four of these spells have a set duration
for 15 seconds, which are indicated with an hourglass:
* FIRE <img src = "https://user-images.githubusercontent.com/90282143/167449483-507bf543-18f2-46bc-ba14-743009907889.png" width="10" height="19"> <br />
* JUMP <img src = "https://user-images.githubusercontent.com/90282143/167449483-507bf543-18f2-46bc-ba14-743009907889.png" width="10" height="19"> <br />
* LIFE
* SHIELD <img src = "https://user-images.githubusercontent.com/90282143/167449483-507bf543-18f2-46bc-ba14-743009907889.png" width="10" height="19"> <br />
* SPELL <img src = "https://user-images.githubusercontent.com/90282143/167449483-507bf543-18f2-46bc-ba14-743009907889.png" width="10" height="19"> <br />


The spell system is derived from "Zelda II: The Adventure of Link". To see how the spell system works in more detail, open the console by pressing tilde (~) and type 'spell'. You should see the following:

![image](https://user-images.githubusercontent.com/90282143/167384279-6d75a20f-bcda-46b4-b44b-cd8a1915de70.png)

The player starts off with 64 magic points, the default amount that Link has in the beginning of Zelda II. Each spell will be occupied with a description, 
followed by in-game screenshots to showcase their functionality.

## FIRE <img src = "https://user-images.githubusercontent.com/90282143/167382004-8b1d88ab-ee59-43b0-8a20-acf9e109cf5a.png" width="30" height="30">
The 'fire' spell allows the player to shoot fireballs out of the sword from a distance. 
In Quake II, the particles shot from the BFG are used to portray Link's fireballs.

Default: <br />
<img src = "https://user-images.githubusercontent.com/90282143/167382923-dfedd679-be14-4973-8d2c-77a94f51ab26.png" width="500" height="375">

Spell Activation: <br />
<img src = "https://user-images.githubusercontent.com/90282143/167382959-cb24e929-e7c1-44cf-bc93-f7c8a4f3253a.png" width="500" height="375">


## JUMP <img src = "https://user-images.githubusercontent.com/90282143/167382084-c84b827e-3c2e-4493-9367-c8a013777c59.png" width="30" height="30">
The 'jump' spell makes the player jump twice as high as before. It also increases the width span of the player's jumps, meaning that jumps will cover 
more horizontal distance.

Default: <br />
<img src = "https://user-images.githubusercontent.com/90282143/167383016-97169ca9-d450-4eb2-828d-a36c371139c3.png" width="500" height="375">

Spell Activation: <br />
<img src = "https://user-images.githubusercontent.com/90282143/167383034-3ef9360b-a048-472f-9156-e57c0a67985c.png" width="500" height="375">


## LIFE <img src = "https://user-images.githubusercontent.com/90282143/167382152-a0e2681c-ab39-4cd4-b222-6c0e14fd112d.png" width="30" height="30">
The 'life' spell recovers some of the player's health (by 50 to be exact). It has the highest magic cost out of all the spells.

Health recoveries will not exceed the maximum health value defined by the game, which is 100. For example, imagine a scenario where the player wants to use 
this spell at 70 health points. Since the player's maximum health cannot exceed 100, the amount of health the player gets back after using the spell can be 
obtained with this formula:

heal_amount = max_health - curr_health
100 - 70 = 30

Therefore, the player will only restore 30 health points instead of 50.


## SHIELD <img src = "https://user-images.githubusercontent.com/90282143/167382190-465c2211-7efb-4085-8762-a66ba86080aa.png" width="30" height="30">
The 'shield' spell is an ability that increases the player's defensive abilities. It reduces the damage the player takes by half. 
Enemy fire, self-damage from inventory weapons, fall height, etc.

Example Scenario: player holds grenade in their hand

Default: <br />
<img src = "https://user-images.githubusercontent.com/90282143/167383071-265c1f3b-2099-41ec-8349-c11dbb7a61a9.png" width="500" height="375"> <br />
Here, the player takes 58 damage.

Spell Activation: <br />
<img src = "https://user-images.githubusercontent.com/90282143/167383283-a1395705-3557-4ced-a0e4-ca6c0d6f3351.png" width="500" height="375"> <br />
Here, the player takes 29 damage.


## SPELL <img src = "https://user-images.githubusercontent.com/90282143/167382237-f227cb8d-26da-4651-8207-a27b06f1cb67.png" width="30" height="30">
The 'spell' spell allows the player to turn several enemies into Barracuda Sharks, which are the Quake II equivalent of the 'Bot' enemies. The railgun has been modified to work with this spell in mind. Whenever a slug shot from the railgun comes into contact with any enemy entity, it will transform into a Barracuda Shark. The Barracuda Shark will sustain damage once the spell is deactivated. This spell works to varying success. <br /> <br />
<img src = "https://user-images.githubusercontent.com/90282143/167652283-18d7fec3-2771-4aa8-aec7-ffb7630c274a.png" width="500" height="375"> <br />


## Shop + Rupees <img src = "https://user-images.githubusercontent.com/90282143/167382384-d466392a-c149-46f1-95a4-29adc6c9d09b.png" width="24" height="30">
Enemies drop rupees on death. Armor shards are used as placeholders for rupees. Each armor shard is worth one rupee.

<img src = "https://user-images.githubusercontent.com/90282143/167382736-60e21b45-bc91-41dc-a783-2eb67ef0d7d1.png" width="500" height="375">
<img src = "https://user-images.githubusercontent.com/90282143/167382763-f469b9cc-4ba9-49c2-a9dc-e2af258458ce.png" width="500" height="375">

The shop has not been fully implemented yet.

## 3 types of functional armor
Only one armor type has been worked on, although not fully implemented yet
* Zora Tunic ~ allows player to breathe underwater

## Other Changes
* Player marine voice lines replaced with Link voice lines ripped from these games:
  * The Legend of Zelda: Ocarina of Time
  * Super Smash Bros. Melee
* Custom sound effects for rupee collecting and spell activation
* Duration-based spells and rupees include UI elements that are fully functional in-game
* "Easy" mode damage scaling has been removed
