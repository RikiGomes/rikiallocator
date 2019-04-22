I made the allocator completely based on shanapu's one. All credit to him

Riki's Weapon Allocator for splewis retakes
## Authors ##
>**Original Developer** - Thomas - [shanapu](https://github.com/shanapu)

>**This Variation Developer** - Riki Gomes - [Riki](https://github.com/RikiGomes)

## How to Install ##
> Move the 'retakes_rikiallocator.smx' into 'csgo/addons/sourcemod/plugins/' folder.

> Move the 'retakes_rikiallocator.phrases.txt' into 'csgo/addons/sourcemod/translations/' folder.

>> **OPTIONAL** Move the files in the 'scripting' folder into 'csgo/addons/sourcemod/scripting' folder.

## About ##
This weapon allocator simulates different kinds of rounds - FULLBUY, FORCEBUY, PISTOL, (DEAGLE).
These rounds will be set through two different modes. 
Ascending rounds (mywa_rounds_chance 1) - first x rounds will be PISTOL, then x FORCEBUY rounds after that x FULLBUY rounds.
Random rounds by chance (mywa_rounds_chance 0) - It's a random chance to play FULLBUY, FORCEBUY, PISTOL & DEAGLE rounds in no special order.
DEAGLE rounds are only available on random rounds (mywa_rounds_chance 0) & don't give grenades.

Player can choose their preferred weapons for these rounds through !gun menu.
The menu is devided in several categories (Pistol Round, Primary, etc.). If you only want to change one weapon type you don't have to go through the sequencial menu as before.

The plugin will give equipments (grenades, armor & kit) in these rounds based of the configured money, mode & max amount of grenades.

This plugin increases the AWP and SSG percentage to the VIP players (in this case assuming the CUSTOM6 flag).
