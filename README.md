# Linux Server Files/Windows Server Files
>last edited:2019/9/21
* <b>SourceMod 1.9.0-git6251</b> by AlliedModders LLC
* <b>MetaMod 1.10.7-git966</b> by AlliedModders LLC
* <b>stripper 1.2.2-hg82</b> by BAILOPAN
* <b>l4dtoolz 1.0.0.9f</b> for windows, <b>1.0.0.9r1</b> for linux (by ivailosp)
* <b>DHooks 2.2.0-detours9</b> by Dr!fter
* <b>Left 4 Downtown 0.4.7.5</b> (windows file by raziEiL, linux file by Spirit_12)
* <b>dosprotect 1.0.0.0v</b> (linux broken) by ZombieX2.net
* <b>tickrate 1.4</b> (up limit: 100tick) by Spirit_12
* <b>GameRules Tools 1.0</b> by psychonic
* <b>voicehook.ext 2.0</b> by Accelerator74

**Step 1:** A [clean L4D1 Dedicated Server](https://github.com/fbef0102/L4D1-Server4Dead/blob/master/README.md#how-to-download-l4d1-dedicated-server-files).

**Step 2:** Choose [Windows Server files](https://github.com/fbef0102/L4D1-Server4Dead/releases/download/v2.0/Windows_Server_files.zip) or [Linux Server files](https://github.com/fbef0102/L4D1-Server4Dead/releases/download/v2.0/Linux_Server_files.zip)(depending on the operating system of your server), and place the files provided in the correct folder.

**Step 3:** Change the Launch Parameters.
  * -console -game left4dead -tickrate 100 +log on +map l4d_vs_airport01_greenhouse +exec server +sv_lan 0

**Step 4:** Adjust your server.cfg to match your rates accordingly.  
For example: For 100 Tickrate, you'd want these settings:

sm_cvar sv_minrate 			"100000"  
sm_cvar sv_maxrate 			"100000"  
sm_cvar sv_minupdaterate 		"101"
sm_cvar sv_mincmdrate 			"101"  
sm_cvar sv_maxupdaterate 		"101"  
sm_cvar sv_maxcmdrate 			"101"  
sm_cvar sv_client_min_interp_ratio 	"0"  
sm_cvar sv_client_max_interp_ratio 	"2"  
sm_cvar rate				"100000"  
sm_cvar net_splitrate			"3"  
sm_cvar net_splitpacket_maxrate		"30000"  
sm_cvar net_compresspackets_minsize 	"32"  
sm_cvar fps_max                         "0"  

# How to download L4D1 Dedicated Server files:
**Warning: Don't try to download "Left 4 Dead Dedicated Server" from steam library, it's broken!! Use steamcmd instead.**

**Step 1:** download [steamcmd](https://developer.valvesoftware.com/wiki/SteamCMD).

**Step 2:** launch steamcmd , steamcmd would automatically download required files .

**Step 3:** after it says "Loading Steam API...OK.", type
* login anonymous
* force_install_dir ./l4d1/
* app_update 222840 validate

**Step 4:** finish downloading and quit.

# Sourcemod Anti-Cheat
[Sourcemod Anti-Cheat Wiki home](https://bitbucket.org/anticheat/smac/wiki/Home)
* smac + smac_aimbot + smac_autotrigger + smac_client + smac_commands + smac_eyetest + smac_rcon + smac_speedhack + smac_spinhack + smac_cvars

# Others
* <b>[L4D1-Competitive-Plugins](https://github.com/fbef0102/L4D1-Competitive-Plugins)</b>: Setup your own L4D1 Servers.
* <b>[Rotoblin-AZMod](https://github.com/fbef0102/Rotoblin-AZMod)</b>: A Competitive L4D1 Versus Configuration
* <b>[L4D1_2-Plugins](https://github.com/fbef0102/L4D1_2-Plugins)</b>: L4D1/2 general purpose and freaky-fun plugins.
