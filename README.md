# RtcwPro

![Alt tag](Assets/rtcwpro.png?raw=true "Title")

Return to Castle Wolfenstein Mod - based on OSPx/xMod (created by Nate) with additions from RtcwPub, ioRtcw, Enemy Territory, ETPub, and other Q3 mods

Main objective: create a competition mod similar to OSP with updates for tournaments and pugs

[b]New features[/b] added that are not in OSP:
 - 1.0/1.0.1
   - corrected head hitboxes (RtcwPub port)
   - faster PK3 downloads (ioRtcw port)
   - unlag antilag
   - antiwarp
   - player HUD names during spectating
   - updated statistics
   - global level server configuration (ET port)
   - server cvar restrictions (ET port)
   - sv_fps fix for flamethrower
   - allow teams feature for ET map porting (i.e. specific team can open doors with lock)
   - minimizer using "minimize" console command
 
 - 1.1 [changelog](changelog/1.1-changelog.txt)
   - dead bodies cannot grab spawn flags
   - specatator freecam can select a player by aiming at them and pressing +attack
   - JSON stat files created for web stats (in progress)
 
 - 1.1.1 [changelog](changelog/1.1.1-changelog.txt)
   - UPS meter (cg_drawSpeed)
   - Added headshot damage cvar to help with antilag/hitbox changes (g_hsDamage)
   
 - 1.1.2 [changelog](changelog/1.1.2-changelog.txt)
   - added nopicmip to tree/ivy/truss shaders so high values of picmip will not remove them

 - 1.2 [changelog](changelog/1.2-changelog.txt)
   - Release 1.2 includes custom client (wolfMP.exe) to allow cvar restrictions, http downloads, and many other features
   - various renderer and overflow fixes
   - add http downloads: cl_wwwdownload, sv_wwwdownload, sv_wwwbaseurl
   - add new resolutions (r_mode): /modelist
   - skybox fixes, clamping etc
   - add r_bloom (demo only)
   - add r_textureanisotropy
   - new flaring, r_flareCoeff etc
   - reduce only non-radius damage knockback
   - fix knockback issues during revives
   - restore revive boosting
   - fix clients hanging on level change
   - fix vote exploits: suicide etc
   - userinfo exploit fixes
   - nuke string fixes
   - add ipv6 support
   - reworked respawn server: safer transitions
   - add new menu script handling
   - add mouse wheel scrollable server list
   - default primitives to 2
   - equalize default values for most cvars with pb cvar list
   - fix download exploit
   - add custom spawn of entities: fs/maps/mapname.spawns
   - add raw mouse input: /in_mouse 2 /in_restart
   - add json stats generation
   - post json stats to remote url: g_stats_curl_submit
   - fix pause limits
   - add additional pause info on pause
   - fix crash on callvote map during pause
   - add new colors and add support for them in console
   - fix ref's status during pause
   - fix obj disappearing into map geometry
   - fix players collision into world: related to the above (very old vanilla bug)
   - add comprehensive cvar restriction: sv_gameconfig <filename> or /config <filename>
   - thread stats submission and other curl calls to avoid lag
   - fix dynos moving during pause
   - remove /r_wolffog from cheat protected cvars
   - add cg_hitsounds and g_hitsounds: latter controls it
   - add new country flags
   - add new logo
   - remove SP asset stuff
   - add challenge validation on the server side
   - add UDP filtering on the server side to prevent common flood attacks against servers
   - fix team overlay with teams greater than teammaxoverlay
   - fix crash with stats related to dyno splash damage
   - fix incorrect dyno defused print for defending team dynos
   - fix player muting
   - fix pause-game clock related issues
   - fix /handicap bugs: removed the command altogether
   - fix random player class changes
   - fix demo view options, third person etc
   - add TAB <key> value expansion in console for current cvar values
   - fix infinite load screens during map change
   - fix num maps limit on the server side: tested with 100
   - fix taking damage from world during pause
   - unlatch com_maxfps so it doesn't need vid_restart
   - add autoexec_mapname on the client side: e.g. main/autoexec_mp_ice.cfg
   - add enemy timer: /timerset <seconds>
   - fix panzer/instant gib damage issues
   - add g_spawnOffset for spawn time offset between teams: random between 1 and cvar integer - 1
   - refactor antilag to rewind more accurately
   - fix revive anim bug
   - auto s_stop for K_SPACE while watching demos
   - default /com_hunkmegs to 256
   - increase cvar buffer in engine to avoid overflows
   - check if file exists for callvote map in mod
   - add an unload mod button to options > mods
   - fix warmup damage
   - display obj icon for team mates in team overlay
   - new ref command: /ref rename <id>
   - add shoutcaster role /scs <pw>
   - add /ref logout and /scs logout
   - shoutcasters can see dynamite timers above dynos
   - shoutcasters can use /noclip
   - shoutcasters can see obj triggers: cg_drawTriggers
   - shoutcasters can change spectator freecam speed: /specspeed <value>
   - shoutcasters can see both teams' reinforcement time
   - add adjustable console height: con_height 0.1-1 and shortcuts for it e.g. shift+console key and alt+console key
   - toggle bodies grabbing flags: g_bodiesGrabFlags
   - allow join during pause
   - add custom screen shake: g_screenShake
   - default r_mode to 6

If you have any questions/comments/concerns then feel free to reach out to us on Discord: https://discord.gg/fn9JVWnbTx

RtcwPro Dev Team
-nihilist, KrazyKaze, Tarator

Contributions from Nate, Dutchmeat, Nobo, S4NDM4NN, and Spaztik
Additional credits for public code: Nico, suburb, the OpenJK dev team.
Installer powered by Advanced Installer: https://www.advancedinstaller.com/
