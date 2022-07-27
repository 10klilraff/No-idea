# eratohoTW - TRANSLATION BRANCH, SCROLL DOWN AND READ THIS
This is the pure translation branch of eratohoTW.
**All** translation of normal lines go here. They will then be ported over to the Game/Master branch, meaning the Game/Master branch has to be written and coded to conform to Game/Translation.

## Branch Purpose
Merging updates from the Japanese to a modded English game is hell. Thus, this branch will only contain translations with a bare minimum of modding.
- No HTML-printing talents
- No custom save menu
- No cheat menu
- No bug fixes

## Translation standards
To keep the game consistent, there are some standards that **you will not break.**
- The game is in second person, ongoing tense. If characters use third-person name and honorifics, keep it since this is touhou after all.

## Coding standards
To make merging in updates not hell, coding has to be done with minimal intrusion.
- **DO NOT** comment out lines and keep them. If you translate a line **remove it**.
- If Japanese grammar is used to achieve tricks, **do not change the code itself**. If this is impossible, create a new function with the same name as the one with the line you were trying to translate, let's say COM100, then make a COM100_TR in a file in the *TRANSLATION* folder and put it there, and have COM100 call COM100_TR then return.
