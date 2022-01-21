# suddenQuake - v.0.3.3
![suddenQuake](https://github.com/Suddendeath-qw/suddenQuake/raw/main/s.png)  
The best quakeworld repository in the wörld.

## Install
1. Find and copy your `pak1.pak` to `id1/pak1.pak`
2. Download latest `ezQuake` from http://www.ezquake.com/downloads.html 
   - _I recommend getting the "Latest development version" or Nightly build_
3. Put `ezQuake.exe` in this folder and run it.


## Configure
1. Start by making sure your `qw/autoexec.cfg` has `exec suddenconfig.cfg` in it.
2. Edit configurations to your liking.

## General - suddenconfig.cfg
This config handles execution of the other parts and acts as a place for key bindings etc.  
alias `+net_scores` shows netgraph and scoreboard at the same time.  
alias `vol+`/`vol-` increases or decreases volume by 0.01.  
Basic movement keys is exactly what it sounds like. Forward, Left, Right, Back, Jump.  
You can alternative use `+jumpreport` instead of `+jump`, this will report status after each 10th jump.  

### Weapon binds 
| alias | description |
| :--- | :--- |
| `+quick_*` | Will fire weapon `*` (sg, ssg, ng, sng, gl, rl, lg) and switch back to shotgun.   |
| `select_*` | Will select weapon to `*` (sg, ssg, ng, sng, gl, rl, lg) be fired with `+select_fire`.  |
| `+select_fire` | Will fire selected weapon (see above) |
| `+rljump` | Fire rl and jump at the same time for optimal height. |

## Teamplay - suddenteamplay.cfg
A teamplay config that is aimed to be lite in both it's messaging and amount of binds. Trying to boil it down to the essentials.  

:shipit: **suddenteamplay.cfg + __s_teamplay.cfg is made so that it can be used in isolation without the rest of suddenQuake package**  
1. Download the latest files
   - https://raw.githubusercontent.com/Suddendeath-qw/suddenQuake/main/qw/__s_teamplay.cfg AND https://raw.githubusercontent.com/Suddendeath-qw/suddenQuake/main/qw/suddenteamplay.cfg
   - OR https://github.com/Suddendeath-qw/suddenQuake/releases/download/v.0.3.3/suddenteamplay.rar
2. Copy `suddenteamplay.cfg` `__s_teamplay.cfg` to your `qw/` folder and `exec suddenteamplay` 
3. Make sure you have `set nick {&cf0fjan&r}` with `f0f` being your color of choice and `jan` being a 3-letter-abbreviation of your name.
4. Open `suddenteamplay.cfg` to edit all of the binds (you can set nick here as well).  
5. `exec suddenteamplay` in console (or preferably in autoexec.cfg)
6. `cfg_save`
7. If you want to update to the latest version of teamplay config you just download `__s_teamplay.cfg` and keep your `suddenteamplay.cfg` for your personal binds etc.

### Teamplay messages
| alias | description |
| :--- | :--- |
| `stp_report` | Reports your current status including health/armor, location, weapon, powerups, need etc.. |
| `stp_point` | Points at an item or enemy, alt. when pointing at teammate shows their status in HUD. |
| `stp_took` | Last taken item, alt. when last item was an powerup, reports team powerup. |
| `stp_killme` | Switch to bestweapon (to drop) and encourage teammates to kill you. |
| `stp_lost` | Location is lost |
| `stp_safe` | Location is safe. |
| `stp_help` | Need help at location |
| `stp_replace` | Replace me at location |
| `stp_coming` | Coming from location |
| `stp_wpkilled` | Enemy weapon killed at location |
| `stp_smart` | Smart report depending on map and location, see below |
| _dm2_ | _Quad/Quad-low: Trick, ng/tele: enemy slipped, big-stairs: coming high with rjump_ |
| _any_ | _Anywhere else reports coming at location_ |

## Quotes! - suddenquotes.cfg
This config is an autogenerated set of memorable quotes from dear members of the Suddendeath clan.  
### Generating the quotes
1. Add your quotes per player in `suddenquotes.json`
2. Run `suddenquotes.exe` or alternatively download https://nodejs.org/en/ and run `node suddenquotes.js` in your `qw/` folder
   - This will generate the `suddenquotes.cfg` config files with all the quote aliases.
### Quote aliases
| alias | description |
| :--- | :--- |
| `q_name_*` | Will say quote #`*` from player with `name`.  |
| `q_name_rand` | Will say a random quote from player with `name`.  |
| `q_rand` | Will say a random quote from any player. |

## Profiles - suddenprofiles.cfg
An easy way to setup all the different team names.    
`// Authentication` - This section is the new auth feature. Read more: https://github.com/ezQuake/ezquake-source/wiki/Authentication  
`// Defaults` - Set your default name, nick, skin etc..  
`// 4on4/2on2/Fakenick` - Create aliases for your alternative profiles  


## New Player model - by CapNBub
CapNBub's created a project to replace all the quake monsters (including player) with new mid-poly models.  
He aims to have very faithful replacements, that also work with the standard MDL limits.  
In order to use this new player model simply rename `qw/progs_new` to `qw/progs`.  
You can find skins for the new model in `qw/skins/newmodel`.

Read more: https://www.quakeworld.nu/forum/topic/6073/new-quake-models


## Icon
![icon](https://github.com/Suddendeath-qw/suddenQuake/raw/main/examples/icon_example.png)  
1. Right-click on your `ezQuake.exe` and select `Create shortcut`
2. Right-click on your shortcut and select `Properties`
3. In the bottom-center click the button `change icon` and select s.ico from this folder
4. Launch Quake using the shortcut
