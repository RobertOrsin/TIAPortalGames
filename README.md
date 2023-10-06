# TIAPortalGames
Some games written in WinCC and VBScript for Siemens Industrial HMIs

These games are done by myself. Assets are scraped from the web or bought from itch.io. Please use only within this project...

As these games are only one during down-time at work and with no intent of sharing, comments are sparse and may make no sense for everybody.

Nothing is done to be done pretty (or even complete). The target for me was to get better with VBS and find limitation of the WinCC environment.

Any use of this code is at your own risk.

If you are stuck and need some advice, feel free to contact me or check the wiki-pages. I update and advance the wiki whenever i find some time.

# Requirements
Siemens TIA Portal V16, with Siemens Step7 Professional and WinCC Advanced.


# Implementation

Each game consists of a list of vars, some scripts and a pop-up-screen. Copy all this into your project and you are set.

Some games need Delay-Timers to be playable (animation-frames, input-lags and so on). You need different delay-values for Simulation and real hardware. You need to fiddle around with them to find a playable gamespeed.

# The Games
## Snake
The classic snake-game.
### Known Bugs and Issues
- Snake does not eat itself
- Games "ends" after 30 apples

## TicTacToe Extreme
Nine TicTacToe-Games combined to a big game. Placing within a game determines where the next player can play. Check the ingame text..
### Known Bugs and Issues
- Winnerscreen shows wrong player

## Viergewinnt (four wins)
A quick and dirty version of four-wins, no winner determination, just placing gamepices.
### Known Bugs and Issues
non so far

## Gameboy Zelda
As the title says, some tiles and sprites to create a gameboy like rpg game. This is so most complex so far and needs more documentation.
Players can push statues around to solve puzzles, slay enemies with sword and bombs.
The Levelfile contains 13 Levels and can be advanced.
There is a boss-fight which needs some more mechanics to be good.
### Known Bugs and Issues
Many...
### Other
Sleepvalues can be configured within/before the game. Values that worked for me:
- Bomb-detonation:  PC: 400; HMI: 8000
- Enemy-Sleeptimer: PC: 120; HMI: 600
- Enemy-Commandtimer: PC:600; HMI: 3600
- Player-DelayTimer:  PC: 5; HMI 120

## Gameboy RPG (Pokemon)
Based of my knowledge from the zelda-game i advanced the map with scrolling. Added a different tile-set (pokemon red/blue) and currently work on it.

Here a snapshot of what is already doable:
![GIF](https://user-images.githubusercontent.com/39116976/158162100-f439914d-0bef-41ee-a1dd-4f85f5cb2a66.gif)


### Features so far included:
- Systemintro
- Gameintro
- reading signs
- starting pokemonbattles in high gras
- includes graphicslists for pokemonsprites and main-battle-screen
- data for all gen. 1 moves
- formula for damage-calculation
- adding stats for all pokemon
- pokemin-inventory (6 pokemon)
- 
### currently worked on
- adding stuff for leveling stats and stat-calculation
- rearanging pokemon and showing the detail-window
- battle-function
  - attack-animation + damage-dealing(-calculation)

## Tetris
Heavy work in progress, nothing to write home about.
