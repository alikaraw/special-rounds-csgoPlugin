# special-rounds-csgoPlugin
A plugin designed to make rounds in community csgo more fun.
Originally posted [here](https://forums.alliedmods.net/showthread.php?t=314977).

## Description:
This plugin is like smillar to how events in "jailbreak" work. In each round, there's a chance for a "special round" to occur.

## Special Rounds List:
In modes with the symbol "✭" you cant pickup weapons and the player can only use the weapon he spawned with, and you cant use the buyzone.
* HeadShot Only // You can only kill players by HeadShotting them
* Random HP // Sets everyone health to a random amount of HP
* Knives Only // The only weapon that deals damage is a knife // ✭
* Shotguns Only // Gives eveyone a random Shotgun // ✭
* Rifles Only // Gives eveyone a random Rifle // ✭
* Pistols Only // Gives eveyone a random Pistol // ✭
* SMGs Only // Gives eveyone a random SMG // ✭
* Space Round // Low gravity with scouts only // ✭

## Requirements:
#include \<sdkhooks>

## ConVars:
* sr_Enable // 0 = Disable , 1 = Enable //  DEFAULT : 1
* sr_Chance // The chance of activating special round // Min : 0 , Max : 100 // DEFAULT : 25
* sr_Gravity // Sets the gravity for the space day // Min : 0.0 , Max : 1.0 //  DEFAULT : 0.5
* sr_MaxHealth // Set the max amount of health you can get in Random HP round //  DEFAULT : 200
* sr_MinHealth //  Set the min amount of health you can get in Random HP round //  DEFAULT : 50
* sr_wzeus // Whether in "knifes only" mode there is also zeus // DEFAULT : 0
NOTE : The value of  sr_MaxHealth needs to be bigger than sr_MinHealth.

## Commands:
### All-Users Commands:
* sm_srinfo // Opens menu with all the special rounds and information on each one.
* sm_srmode // Says what mode is currently active in this round.
* sm_srversion // Says what is the current virsion of the plugin is in the server.

### Admins Commands:
* sm_srset // Enable and disable certain modes.
* sm_srforce // Force a special mode to get started next round.
* sm_srsave // Save the currect settings.
* sm_srload // Load the last settings that was saved.

## Files:
The plugin will create a folder with a database to save the settings of the plugin.
Path : addons\sourcemod\data\SpecialRounds
