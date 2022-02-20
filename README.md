# If you appreciate my work, you can [PayPal Donate](https://paypal.me/Harry0215?locale.x=zh_TW) me.
> Click [HERE](https://github.com/fbef0102/L4D1-Server4Dead/releases) to download package
# Linux Server Files/Windows Server Files
* <b>SourceMod 			1.10-git6528</b> 	    by AlliedModders LLC
* <b>MetaMod 			1.11-git1145</b> 	    by AlliedModders LLC
* <b>stripper 			1.2.2-git129</b> 		by BAILOPAN
* <b>l4dtoolz 			1.1.0.1</b> 		    by ivailosp、Accelerator74
* <b>DHooks 			2.2.0-detours17</b> 	by Dr!fter、Peace-Maker
* <b>Tickrate Enabler	1.5</b> 	    		by ProdigySim、Spirit_12、Accelerator74
* <b>VoiceHook	 		3.0</b> 	    		by Accelerator74
* <b>geoipcity 			1.1.2</b> 				by GoD-Tony
* <b>REST in Pawn		1.3.1</b>				by ErikMinekus
* <b>socket				3.0.2</b>				by sfPlayer & JoinedSenses
* <b>sourcescramble 	0.7.0</b> 				by nosoop
* <b>CollisionHooks	 	0.2(linux only)</b> 	by VoiDeD、Spirit_12
# Server Install
**Step 1:** A [clean L4D1 Dedicated Server](https://github.com/fbef0102/L4D1-Server4Dead/blob/master/README.md#how-to-download-l4d1-dedicated-server-files).

**Step 2:** Choose [Windows Server files](https://github.com/fbef0102/L4D1-Server4Dead/releases/download/v4.0/Windows_Server_files.zip) or [Linux Server files](https://github.com/fbef0102/L4D1-Server4Dead/releases/download/v4.0/Linux_Server_files.zip)(depending on the operating system of your server), and place the files provided in the correct folder.

**Step 3:** Adjust your **server_rates.cfg** to match your rates accordingly.  
* For 100 Tickrate, you'd want these settings:
>sm_cvar sv_minrate 			"100000"

>sm_cvar sv_maxrate 			"100000"

>sm_cvar sv_minupdaterate 		"101"

>sm_cvar sv_maxupdaterate 		"101"

>sm_cvar sv_mincmdrate 			"101"

>sm_cvar sv_maxcmdrate 			"101"

>sm_cvar rate				"100000"

>sm_cvar net_splitpacket_maxrate "50000"

>sm_cvar fps_max    "0"


**Step 4:** Change the Launch Parameters.
  * -console -game left4dead -tickrate 100 +log on +map l4d_vs_airport01_greenhouse +exec server +sv_lan 0

# How to download L4D1 Dedicated Server files:
**Warning: Don't try to download "Left 4 Dead Dedicated Server" from steam library, it's broken!! Use steamcmd instead.**

**Step 1:** download [steamcmd](https://developer.valvesoftware.com/wiki/SteamCMD).

**Step 2:** launch steamcmd , steamcmd would automatically download required files .

**Step 3:** after it says "Loading Steam API...OK.", type
* force_install_dir ./l4d1/
* login anonymous
* app_update 222840 validate

**Step 4:** finish downloading and quit.

# Sourcemod Anti-Cheat
> [SMAC Wiki](https://github.com/Silenci0/SMAC/wiki)

> [SMAC 0.8.7.3 fork](https://github.com/Silenci0/SMAC)
* smac + smac_aimbot + smac_autotrigger + smac_client + smac_commands + smac_cvars + smac_rcon + smac_speedhack + smac_spinhack

# Others
* <b>[L4D1-Competitive-Plugins](https://github.com/fbef0102/L4D1-Competitive-Plugins)</b>: L4D1 Competitive enhancement, bug/glitch fixes, general purpose and freaky-fun plugins.
* <b>[Rotoblin-AZMod](https://github.com/fbef0102/Rotoblin-AZMod)</b>: A Competitive L4D1 Versus Configuration
* <b>[L4D1_2-Plugins](https://github.com/fbef0102/L4D1_2-Plugins)</b>: L4D1/2 general purpose and freaky-fun plugins.
