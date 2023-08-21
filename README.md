# Special Rounds | CS:GO Plugin
A plugin designed to make rounds in community csgo more fun.
Originally posted [here](https://forums.alliedmods.net/showthread.php?t=314977).

## Description:
This plugin is like smillar to how events in "jailbreak" work. In each round, there's a chance for a "special round" to occur.

## Special Rounds List:
|Name|Description|Only Given Items|
|-----|------|-----|
|HeadShot Only| You can only kill players by HeadShotting them| False|
|Random HP|Sets everyone health to a random amount of HP|False|
|Knives Only|The only weapon that deals damage is a knife |True|
|Shotguns Only|Gives eveyone a random Shotgun|True|
|Rifles Only|Gives eveyone a random Rifle |True|
|Pistols Only|Gives eveyone a random Pistol|True|
|SMGs Only|Gives eveyone a random SMG|True|
|Space Round|ow gravity with scouts only|True|

NOTE : "Only Given Items" means the player can only use the items given to him at the beginning of the round

## Requirements:
#include \<sdkhooks>

## ConVars:
|Name| Description | values | Default |
|----|------|------------|-------|
|sr_Enable| Toggles the plugin | 0 OR 1| 1 |
|sr_Chance|  The chance of activating a special round |0 <= x <=100| 25 |
|sr_Gravity| The gravity for the space day|0.0 <= x <= 1.0 | 0.5 |
|sr_MaxHealth|The max amount of health you can get in Random HP round| - | 200|
|sr_MinHealth|The min amount of health you can get in Random HP round| - | 50|
|sr_wzeus|Whether in "knifes only" mode there is also zeus|0 OR 1| 0|

NOTE : The value of sr_MaxHealth needs to be bigger than sr_MinHealth

## Commands:
### All-Users Commands:
|Command|Description|
|-------|-----------|
|sm_srinfo|Opens menu with all the special rounds and information on each one|
|sm_srmode|Shows what mode is currently active in this round|
|sm_srversion|Shows what is the current virsion of the plugin is in the server.|

### Admins Commands:
|Command|Description|
|-------|-----------|
|sm_srset|Enable and disable certain modes|
|sm_srforce|Force a special mode to get started next round|
|sm_srsave|Save the currect settings|
|sm_srload|Load the last settings that was saved|

## Files:
The plugin will create a folder with a database to save the settings of the plugin inside ```addons\sourcemod\data\SpecialRounds```
