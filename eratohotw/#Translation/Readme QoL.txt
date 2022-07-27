This file contains documentation for the changes QoL does.
QoL contains the following branches:
 - html-talents
 - ignore-stable-period-restrictions
 - malehus
 - navigation
 - random-chara
 - virgin-settings
Along with other small things that have been added over time. More documentation to come.


Html-talents
Makes the player able to see talent descriptions by hovering over them. Relevant files are in ERB/TRANSLATION/HTML_TALENTS
It makes PRINT_STATE_TALENT run PRINT_STATE_TALENT_MOD and then return.
Merged in d20c0ec437d23f2973b3c2922360f700df8b6863

Ignore-stable-period
Normally you can't have sex if the pregnancy is less than 30 days old, or older than 71. This fixes that.
Uses a flag to disable some checks.
Merged in d285ab1d3786ddb403c8150b0712fe74f904818e

Malehus
The game expects everyone but the player to be male. So far I've only found one instance where it explicitly confirms the gender without checking - during peeping. 
Currently just a few lines in NASIKUZUSI.ERB
Merged in a8e68012c3b56e8131e5dd927f56d9e44709fedf

Navigation
Allows you to see all areas you can go to on the map, rather than just the adjacent ones.
Also makes "whereabout sense" less of an absolute requirement. Lets you see if people are in adjacent areas. 
Merged in 84322ba221c15e75d3a8194f76455e22a6298877

Random-chara
Lets you revisit random characters.
Merged in 5b82f24f843c3dc782cdf693620c5cdea28516a6
Now rendered useless as this has been added to the base game.

Virgin-settings
Lets you choose more settings at the start of the game, including random values (for instance 30% forced virgins, 70% default).
Merged in 164358abebe966ef65d4c478baabefd194b860c1

Slip out of pushed down 31/8/2018
If you have more than 500 tsp you can slip out when pushed down by simply exhausting the target, effectively ending the encounter.
ERB\コマンド関連\COMF\COMF850 抜け出す.ERB
52~

Buy additional fields 8/11/2018
Allows the player to buy additional field slots(up to a maximum of 5) at the flower shop in the shopping district of the human village.
ERB\コマンド関連\COMF\外出系\COMF618 花屋.ERB
17 lines added, 1 modified

Whereabout sense expansion
Changes HITOSAGASI to accept a second argument, which prints "other areas" when searching.

Ability tooltip
ERB\TRANSLATION.ETB 
984
Alternate abilities display that uses HTML to get tooltips.

15/4/2020
They moved things to that NEWGAME folder, so QoL got reshuffled a bit.

22/5/2021
YASAI - 水やり代行 flag prevents fields from drying