MyWeaponAllocator

MyWeaponAllocator for splewis retakes - https://forums.alliedmods.net/showthread.php?t=262658

## Authors ##
>**Original Developer** - Thomas - [shanapu](https://github.com/shanapu)

>**Modifications and Maintenence Developer** - Riki Gomes - [Riki](https://github.com/RikiGomes)

This weapon allocator simulates different kinds of rounds - FULLBUY, FORCEBUY, PISTOL, (DEAGLE).
These rounds will be set through two different modes. 
Ascending rounds (mywa_rounds_chance 1) - first x rounds will be PISTOL, then x FORCEBUY rounds after that x FULLBUY rounds.
Random rounds by chance (mywa_rounds_chance 0) - It's a random chance to play FULLBUY, FORCEBUY, PISTOL & DEAGLE rounds in no special order.
DEAGLE rounds are only available on random rounds (mywa_rounds_chance 0) & don't give grenades.

Riki's updated version of the plugin will give you different pistols at Pistol Round and during Buy Rounds.

Player can choose their preferred weapons for these rounds through !gun menu.

The plugin will give equipments (grenades, armor & kit) in these rounds based of the configured money, mode & max amount of grenades.

Take a look at the configuration for a better understanding.


```
// 0 - disabled, 1 - enable plugin
// -
// Default: "1"
// Minimum: "0.000000"
// Maximum: "1.000000"
mywa_enable "1"

// 0 - chance / 1- rounds
// -
// Default: "1"
// Minimum: "0.000000"
// Maximum: "1.000000"
mywa_rounds_chance "1"

// percent chance a round will be a pistol round (mywa_rounds_chance 0)
// -
// Default: "20"
// Minimum: "0.000000"
mywa_chance_pistol "20"

// percent chance a round will be a force round (mywa_rounds_chance 0)
// -
// Default: "30"
// Minimum: "0.000000"
mywa_chance_force "30"

// percent chance a round will be a deagle round (mywa_rounds_chance 0)
// -
// Default: "5"
// Minimum: "0.000000"
mywa_chance_deagle "5"

// how many round will be pistol round (mywa_rounds_chance 1)
// -
// Default: "3"
// Minimum: "0.000000"
mywa_rounds_pistol "3"

// how many round will be force round (mywa_rounds_chance 1)
// -
// Default: "4"
// Minimum: "0.000000"
mywa_rounds_force "4"

// money for weapons and equipment on fullbuy round
// -
// Default: "16000"
// Minimum: "0.000000"
mywa_money_full "16000"

// money for weapons and equipment on pistol round
// -
// Default: "800"
// Minimum: "0.000000"
mywa_money_pistol "800"

// money for weapons and equipment on forcebuy round
// -
// Default: "2700"
// Minimum: "0.000000"
mywa_money_force "2700"

// min number of player in terrorist team before AWP is available for T
// -
// Default: "3"
// Minimum: "1.000000"
mywa_awp_min_t "3"

// min number of player in terrorist team before scout is available for T
// -
// Default: "2"
// Minimum: "1.000000"
mywa_scout_min_t "2"

// max number of AWPs for terrorist team / 0 - no AWPs
// -
// Default: "1"
// Minimum: "0.000000"
mywa_awp_t "1"

// max number of scouts for terrorist team in force rounds/ 0 - no scouts
// -
// Default: "1"
// Minimum: "0.000000"
mywa_scout_t "1"

// max number of molotovs for terrorist team / 0 - no molotovs
// -
// Default: "2"
// Minimum: "0.000000"
mywa_molotov_t "2"

// max number of smokegrenades for terrorist team / 0 - no smokegrenades
// -
// Default: "2"
// Minimum: "0.000000"
mywa_smoke_t "2"

// max number of flashbangs for terrorist team / 0 - no flashbangs
// -
// Default: "3"
// Minimum: "0.000000"
mywa_flash_t "3"

// max number of HEgrenades for terrorist team / 0 - no HEgrenades
// -
// Default: "3"
// Minimum: "0.000000"
mywa_he_t "3"

// min number of player in counter-terrorist team before AWP is available for CT
// -
// Default: "3"
// Minimum: "1.000000"
mywa_awp_min_ct "3"

// min number of player in counter-terrorist team before scout is available for CT
// -
// Default: "2"
// Minimum: "1.000000"
mywa_scout_min_ct "2"

// max number of AWPs for counter-terrorist team / 0 - no AWPs
// -
// Default: "1"
// Minimum: "0.000000"
mywa_awp_ct "1"

// max number of scouts for counter-terrorist team in force rounds/ 0 - no scouts
// -
// Default: "1"
// Minimum: "0.000000"
mywa_scout_ct "1"

// max number of molotovs for counter-terrorist team / 0 - no molotovs
// -
// Default: "2"
// Minimum: "0.000000"
mywa_molotov_ct "2"

// max number of smokegrenades for counter-terrorist team / 0 - no smokegrenades
// -
// Default: "2"
// Minimum: "0.000000"
mywa_smoke_ct "2"

// max number of flashbangs for counter-terrorist team / 0 - no flashbangs
// -
// Default: "3"
// Minimum: "0.000000"
mywa_flash_ct "3"

// max number of HEgrenades for counter-terrorist team / 0 - no HEgrenades
// -
// Default: "3"
// Minimum: "0.000000"
mywa_he_ct "3"

// order to buy the equipments / 0 - random, 1 - 1st grenades 2nd armor & kit, 2 - 1st armor & kit 2nd grenades 
// -
// Default: "0"
// Minimum: "0.000000"
// Maximum: "2.000000"
mywa_buy_order "0"

// 0 - disabled, 1 - enable kevlar
// -
// Default: "1"
// Minimum: "0.000000"
// Maximum: "1.000000"
mywa_kevlar "1"

// 0 - disabled, 1 - enable helm
// -
// Default: "1"
// Minimum: "0.000000"
// Maximum: "1.000000"
mywa_helm "1"

// 0 - disabled, 1 - enable defuser
// -
// Default: "1"
// Minimum: "0.000000"
// Maximum: "1.000000"
mywa_defuser "1"

// 0 - disabled, 1 - enable deagle for pistol & fullbuy rounds
// -
// Default: "1"
// Minimum: "0.000000"
// Maximum: "1.000000"
mywa_deagle "1"

// 0 - disabled, 1 - enable revolver for pistol & fullbuy rounds
// -
// Default: "1"
// Minimum: "0.000000"
// Maximum: "1.000000"
mywa_revolver "1"

// 0 - disabled, 1 - enable bombsite notifications
// -
// Default: "1"
// Minimum: "0.000000"
// Maximum: "1.000000"
mywa_bombsite "1"
```
