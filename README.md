# Pokéwars

Description:

Pokéwars is a realtime online multiplayer game made using sprites from Pokemon Leaf Green and Fire Red. 

This project was made using python3.7, pygame and the sockets module to handle incoming connections.

The player must navigate randomly generated maps, gathering weapons and power-ups from long grass and deep pools, and destroy enemy players.

The game supports 7 native maps, each using a range of difference sprites and terrains from Pokémon. 

The Map class in  map_generation.py has generate_map(),save() and load() functions, which can be used to generate and save new maps by passing in a list of sprites. 

The game maps used can be changed by editing maps[] in config.py. Any newly generated maps should be added here.


# Further Game Details

On connection player must enter name, and is then assigned a colour based on their assigned connection ID.

Players can find new weapons and power ups (currently 'bike' and 'mushroom' only) by searching in grass and water.

Navigating through grass and water reduces the players movement speed. 

Bikes 2x the players speed.

Mushrooms 2x the players size - providing temporary immunity to death and the ability to trample other players via contact.

Game statistics are shown in the menu/leaderboard (Z).

Host is considered to be first person connected to the server.

# Controls

Movement: Arrow Keys

Shoot: Spacebar

Strafe: S

Menu/Leaderboard: Z

Show Grid: X

Change Map (Host only): C

# Requirements
- python3.7

- pygame

# How to run

Change HOST and PORT in config.py to reflect your setup.

Ideally place server.py, config.py and leaderboard.py on a server. Create a new database from the leaderboard file. Multiple instances can then be launched from anywhere with many players playing simultaneously.

Another option is to download and use Hamachi to simulate your LAN. 

Only the host player must run server.py. Other players need only run main.py.

# LICENSE

<em>Not for commercial use</em>. Please credit me if you intend to use code from this game.

# Screenshots


![ss1](https://user-images.githubusercontent.com/31314787/75721064-91a95200-5ccf-11ea-9aeb-8bc665aceb04.PNG)
![ss2](https://user-images.githubusercontent.com/31314787/75721066-92da7f00-5ccf-11ea-9a6a-70d7371ccd19.PNG)
![ss3](https://user-images.githubusercontent.com/31314787/75721067-940bac00-5ccf-11ea-838e-cc18b3bb3fd5.PNG)
