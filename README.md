# InfectedCompany
___
![infected_company_banner](https://imgur.com/lpneTX0.png)

> # *NOTE: All players will need the mod installed to play together*

> ## This mod is still in beta. Please report any bugs and issues you encounter while using the mod by creating an issue on the [official GitHub repo issues page](https://github.com/InfectedCompany/InfectedCompany/issues). Thank you!

## Infected Company
- **Trust no-one.** One or more of your crewmates are infected! Trust no-one, collect scrap and survive!
- **New items.** Adds new items to the game: **incendiary grenade**, **infected detector** and **handheld radar**.
- **Quarantine phase.** Can you survive the facility lockdown?
- **Lobby size support.** Compatible with lobby size enhancement mods! The game will scale accordingly.
- **And more!**

![infected_monster_spawn](https://imgur.com/S7LCotU.gif)

## Objectives
### Survivor objective
The survivor's main objective is to collect enough scrap to meet the newly added **round quota** (not to be confused with the *profit quota*).
The round quota is the total value of collected scrap the survivors must meet in a **SINGLE day/round**. 
The round quota will increase along with the normal game's **profit quota**. The survivors win if they're able to meet the round quota and survive.

### Infected objective
The objective is to prevent the survivors from meeting the round quota. You're given many tools to do so such as becoming a monster yourself :)

## Game phases

### Start phase
- You will need at least 3 players in the lobby to start the game. **This value can be configured by the host**
- Once the ship lands, random players in the lobby will be chosen as the infected.
- The more players the lobby has, the more will be chosen as infected. **This value can be configured by the host (default `3.5 players for each infected`)**

### Game phase
- During this phase the game plays like normal, however, someone in your crew is infected.
- The infected will slowly build up **insanity** while they're inside of the facility.
- Once the insanity meter is full, they will have the ability to turn into the infected monster.
- The qurantine phase begins when there is at least a single active infected roaming inside of the facility.

### Quarantine phase
The quarantine phase begins when there is at least a single active infected monster **inside of the facility**,
and ends when they're all neutralized or if the infection/insanity recedes. The facility is put into lockdown mode during the quarantine:

- An alarm and announcer will signal the start and end of the quarantine phase
- Facility entrances and emergency exits are locked
- Teleporters are disabled
- Ship monitors are disabled
- The ship terminal is disabled
- Walkie-talkies are disabled
- Facility lights will switch off and emergency lights will switch on

### Endgame phase and scoring
The game ends when any of the following events occur:

	1. The survivors collect and secure enough scrap to meet the round quota (the survivors win)
	2. All the survivors die (the infected win)
	3. The ship leaves without meeting the round quota (the infected win)



### Ship leaderboard
Player scores will be recorded and displayed on a leaderboard found in the ship.

## Survivor gameplay
- **Panic mode (*default 'p' key*):** Drop all items and gain a temporary speed-boost (60 second cooldown). Use this wisely to escape the infected!
- **Tips against the infected**: 
	- Use flashes and stuns to slow and blind the infected. They cannot kill while stunned.
	- Use the *infected detector* to sniff out who's infected or not.


## Infected gameplay
- **Insanity:** The insanity meter will fill up while you're inside of the facility **(and outside during night-time)**. The rate increases with your fear level, meaning if you see monsters or dead bodies, your insanity will charge faster. Once full, you can turn into the infected monster.
- **Infected mode (*default 'x' key*):** Transform into the infected once your insanity meter is full. While transformed, you will have instant acceleration and the ability to kill players.
- **Infected kill attack (*default 'z' key*):** While in infected mode, you can kill other players by ripping their guts out (30 second cooldown).
- **Immune to monsters:** Other monsters will ignore you while you are in infected mode. Remember, you're immune to monsters, not bullets. Turrets will still attack you!

![infected_despawn](https://imgur.com/v0cttmE.gif)

## New Items

### Infected Detector
- Cannot be bought and must be found as a rare drop within the facility
- Single-use scan, once used it cannot be recharged
- Only the person who used the scan will know the result, this opens up potential deception tactics ;)
- The charge is consumed even if there was nobody within the range of the scan, don't waste it!
- It will only show a positive infected reading if the infected has a high insanity level.

### Handheld Radar
- Can be bought from the terminal for **120 credits**
- Use it wisely! It runs on batteries that last for 150 seconds
- Pings the locations of nearby players and *most* monsters
- Monster and player pings are indistinguishable
- Some monsters will not show up on the radar
- You can pocket the item and leave it on to hear the ping sounds of nearby players and monsters

### Incendiary Grenade
- Can be bought from the terminal for **50 credits**
- The fire from the grenade lasts for 7 seconds and spreads upon impact
- Will damage both players and monsters
- Getting burned will slow you

![incendiary_fire](https://imgur.com/dfdEiKy.gif)

## Gameplay balance changes
Several gameplay balance-changes were made to improve the game's pacing. The following changes have been applied:

	1. Days are 30% longer
	2. Starting quota is 50% higher
	3. New profit quotas will increase with an additional ~15%
	4. Maps are 50% larger and have 50% more scrap
	5. Maps will spawn 25% more monsters

## Host config

| Option | Description |
| ----------- | ----------- |
| `players_per_infected` | Amount of players per infected (min. `1`). For example, if this value is `3.5`, then per `3.5` players, another player will be chosen as an infected. There is always at least `1` infected in the game (default `3.5`)
| `number_of_players_required_to_start` | Amount of players required to start the game (min. `1`) (default `3`)
| `min_round_quota_for_survivor_win` | First round quota that the survivors have to make (default `250`)

## Keybind configuration
If you want to rebind the keybindings, you can do so by modifying the `BepInEx/config/InfectedCompany.InfectedCompany.cfg` file. If you don't see this file then you must **start the game at least once** to generate it.

If you would like to revert the config back to default, just delete the file and restart the game.

| Key      | Config key value example | 
| ----------- | ----------- |
| letters      | a      
| numbers   | 0
| num pad numbers   | num 0   
| function keys | f1
| arrow keys | up/left/down/right
| ctrl | ctrl (or right ctrl)
| alt   | alt (or right alt)  
| shift   | shift (or right shift)  
| space   | space      
| esc   | esc   
| caps lock   | caps lock        
| num lock   | num lock      


## Installation

> *NOTE: All players will need the mod installed to play*

### Thunderstore installation

1. Launch the Thunderstore mod manager
2. Search for the mod and install it (with dependencies)

### Manual installation

1. Install [BepInEx](https://thunderstore.io/package/bbepis/BepInExPack/). This is used to load and run the mod.
2. Download this mod and place the `InfectedCompany.dll` into your `BepInEx/plugins` folder.

## What's next?

### Custom moon with unique level mechanics
- More details coming soon..

### Custom enemies
- Can't have a custom moon without custom enemies :D

### A fully custom game mode
- This game mode will give the survivors and infected objectives in addition to the normal gameplay. Details soon..


## FAQ

### Does this mod work with lobby size modifications?
Yes! In fact, the number of infected scales with lobby size. This is configurable by the host.

### Does everyone need to have the mod installed?
Yes. Otherwise you cannot play together.

### How do I rebind my keys?
See section on [Keybind configuration](#keybind-configuration).

## Report bugs/issues/requests

Please report any bugs and issues you encountered while using the mod or make a request by creating an issue on the [official GitHub repo issues page](https://github.com/InfectedCompany/InfectedCompany/issues). Thank you! :)

### v0.0.9
- Initial release

