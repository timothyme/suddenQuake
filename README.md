# suddenQuake
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

#### Weapon binds 
`+quick_rl` - switch to RL, fire and switch back to shotgun all in one button.  
`select_lg` - select LG to be used when pressing the `select_fire` bind. This will not equip LG.  
`+rljump` - fire rl and jump at the same time for optimal height.

## Teamplay - suddenteamplay.cfg
A teamplay config that is aimed to be lite in both it's messaging and amount of binds. Trying to boil it down to the essentials.  

:shipit: **suddenteamplay.cfg is made so that it can be used in isolation without the rest of suddenQuake package**  
Just `copy suddenteamplay.cfg` to your `qw/` folder and `exec suddenteamplay`  
#### First
Make sure you have `set nick {&cf0fjan&r}` with `f0f` being your color of choice and `jan` being a 3-letter-abbreviation of your name.
#### Teamplay messages
| alias | description |
| --- | --- |
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

