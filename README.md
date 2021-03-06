## <a name="displaygg"></a>Display.gg

### Table of Contents

- [Display.gg](#displaygg)
  - [What is Display.gg?](#what-is-displaygg)
  - [More Details](#more-details)
  - [Information Displayed](#information-displayed)
  - [Player skill? Carry factor?](#player-skill-carry-factor)
- [Windows Instructions](#windows)
  - [Installation](#installation-instructions-windows)
  - [Running](#running-instructions-windows)
- [Mac Instructions](#mac)
  - [Installation](#installation-instructions-mac)
  - [Running](#running-instructions-mac)
- [Statement](#statement)

### <a name="what-is-displaygg"></a>What is Display.gg?
A loading screen display for League of Legends.
<img src='http://i.imgur.com/aiSwuXq.jpg' alt='Demo'></img>
### <a name="more-details"></a>More Details
<font color="lightblue">Display.gg</font> is a python script that you keep running on your computer. It detects when you are loading into a game and pulls up the game's details.
### <a name="information-displayed"></a>Information Displayed
- Game type (CLASSIC, RANKED, ARAM, etc.)
- Summoner name
- Champion
- Summoner spells
- Keystone mastery
- Current season rank
- Runes
- Average ranked KDA on champion
- Win Rate on champion
- Ranked games on champion
- Player skill on champion
- Carry Factor (CF)

### <a name="player-skill-carry-factor"></a>Player skill? Carry factor?
Player skill is split into three categories: ***ONE TRICK***, ***NEW***, and ***NORMAL***. If there is nothing on top of the summoner
name, their skill level is ***NORMAL***. ***ONE TRICK*** means they have played at least **50%** of their ranked games with that
champion, while ***NEW*** means they have played less than **2.5%** of their ranked games with that champion.

Carry factor measures the player's likeliness to carry on a scale from **0.0** (not likely) to **10.0** (extremely likely).
It is calculated by an algorithm that analyzes their win/loss record from the past **10** matched games.

## <a name="windows"></a> Windows Instructions (WARNING: not extensively tested)

### <a name="installation-instructions-windows"></a>Installing
Download and unzip the ZIP file or clone the project into a directory of your choice. Rename the folder to "DisplayGG" or whatever name you want.

Make sure you have Python 3.x installed on your computer. The easiest way to check is by going to Command Prompt and entering:

`python3`

If it says either "command does not exist" or displays a version lower than 3, install the latest 3.x from
[here](https://www.python.org/downloads/). *Remember which of the two commands worked, because you will need it later.*

Make sure you have pip by entering the command

`pip3`

into Command Prompt. If it
gives you a long list of commands, you have it. If not, follow the instructions [here](https://pip.pypa.io/en/stable/installing/).

Navigate to the DisplayGG folder in Command Prompt (For example, if it is in Downloads/DisplayGG, enter "cd ~/Downloads/DisplayGG"). Now enter the following commands (if it prompts you for
  your password, enter it because it needs admin permissions to install):

`pip3 install -r requirements.txt`


Change the values in the config.json file. Where it says "Summoner_Name", enter your summoner name with quotes around it.
You can play around with the scale_factor until you find one that suits your tastes.
*Going under 6 is not
recommended because it will cause visual clashes!*

For region, valid values are:
- br (Brazil)
- eune (Europe North-East)
- euw (Europe West)
- kr (Korea)
- lan (Latin America North)
- las (Latin America South)
- na (North America)
- oce (Oceania)
- tr (Turkish)
- ru (Russia)
- pbe (Public Beta Environment)

*Make sure there are quotes around it. Do not enter the text in parentheses!*


<font color="blue">**Congratulations! Display.gg is installed!**</font>
### <a name="running-instructions-windows"></a>Running
*Replace `x` with either `python` or `python3` depending on which command worked when you were checking your Python version earlier*

In Command Prompt, from the DisplayGG folder, run this command:

`x script.py 0`

You can put a summoner name in double-quotes afterwards if you want the program to load data for a summoner other than the one in your config.json, like so:

`x script.py 0 "SUMMONERNAME"`

Now the program is running and will automatically open when you load into game. You can exit the program from the Command Prompt window by pressing Ctrl-C.

## <a name="mac"></a> Mac Instructions

### <a name="installation-instructions-mac"></a>Installing
Download and unzip the ZIP file or clone the project into a directory of your choice. Rename the folder to "DisplayGG" or whatever name you want.

Make sure you have Python 3.x installed on your computer. The easiest way to check is by going to Terminal and entering:

`python3`

If it says "command does not exist" or displays a version lower than 3, install the latest 3.x from
[here](https://www.python.org/downloads/).

Make sure you have pip by entering the command

`pip3`

into Terminal. If it
gives you a long list of commands, you have it. If not, follow the instructions [here](https://pip.pypa.io/en/stable/installing/).

Navigate to the DisplayGG folder in Terminal (For example, if it is in Downloads/DisplayGG, enter "cd ~/Downloads/DisplayGG"). Now enter the following commands (if it prompts you for
  your password, enter it because it needs admin permissions to install):

`sudo pip3 install -r requirements.txt`


Change the values in the config.json file. Where it says "Summoner_Name", enter your summoner name with quotes around it.
You can play around with the scale_factor until you find one that suits your tastes.
*Going under 6 is not
recommended because it will cause visual clashes!*

For region, valid values are:
- br (Brazil)
- eune (Europe North-East)
- euw (Europe West)
- kr (Korea)
- lan (Latin America North)
- las (Latin America South)
- na (North America)
- oce (Oceania)
- tr (Turkish)
- ru (Russia)
- pbe (Public Beta Environment)

*Make sure there are quotes around it. Do not enter the text in parentheses!*

<font color="blue">**Congratulations! Display.gg is installed!**</font>
### <a name="running-instructions-mac"></a>Running
In Terminal, from the DisplayGG folder, run this command:

`python3 script.py 1`

You can put a summoner name in double-quotes afterwards if you want the program to load data for a summoner other than the one in your config.json, like so:

`python3 script.py 1 "SUMMONERNAME"`

Now the program is running and will automatically open when you load into game. You can exit the program from the Terminal window by pressing Ctrl-C.

### <a name="statement"></a>Statement
Display.gg isn't endorsed by Riot Games and doesn't reflect the views or opinions of Riot Games or anyone officially involved in producing or managing League of Legends. League of Legends and Riot Games are trademarks or registered trademarks of Riot Games, Inc. League of Legends © Riot Games, Inc.
