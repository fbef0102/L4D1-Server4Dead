>click [here](https://github.com/fbef0102/L4D1-Server4Dead/releases) to download package (last edited:2019/11/03)
# Linux Server Files/Windows Server Files
>recommended system **win 10** for windows and **ubuntu** for linux
* <b>SourceMod 			1.9.0-git6251</b> 	    by AlliedModders LLC
* <b>MetaMod 			1.10.7-git966</b> 	    by AlliedModders LLC
* <b>stripper 			1.2.2-hg82</b> 		    by BAILOPAN
* <b>l4dtoolz 			1.0.0.9f</b> 		    by ivailosp
* <b>DHooks 			2.2.0-detours9</b> 	    by Dr!fter、Peace-Maker
* <b>Left 4 Downtown 	0.4.7.5(windows)</b>    by Igor "Downtown1" Smirnov 、 Andrew "XBetaAlpha" Burrows 、 AtomicStryker 、 Michael "ProdigySim" Busby 、 Continued by: sentient & raziEiL, <b>(linux)</b> by Spirit_12
* <b>dosprotect 		1.0.0.0-18(windows)</b> by ZombieX2.net、D1maxa <b>(linux broken)</b>
* <b>tickrate 			1.4(windows)</b> 	    by ProdigySim、Spirit_12, <b>1.44(linux)</b> by Engine、aXe
   * tickrate 1.4(windows) upper limit is **100**, tickrate 1.44(linux) tickate upper limit is **128**
* <b>GameRules Tools 	1.0</b> 			    by psychonic
* <b>voicehook.ext 		2.0</b> 			    by Accelerator74

**Step 1:** A [clean L4D1 Dedicated Server](https://github.com/fbef0102/L4D1-Server4Dead/blob/master/README.md#how-to-download-l4d1-dedicated-server-files).

**Step 2:** Choose [Windows Server files](https://github.com/fbef0102/L4D1-Server4Dead/releases/download/v2.0/Windows_Server_files.zip) or [Linux Server files](https://github.com/fbef0102/L4D1-Server4Dead/releases/download/v2.0/Linux_Server_files.zip)(depending on the operating system of your server), and place the files provided in the correct folder.

**Step 3:** Adjust your **server_rates.cfg** to match your rates accordingly.  
* For 100 Tickrate, you'd want these settings:
>sm_cvar sv_minrate 			"100000"

>sm_cvar sv_maxrate 			"100000"

>sm_cvar sv_minupdaterate 		"101"

>sm_cvar sv_maxupdaterate 		"101"

>sm_cvar sv_mincmdrate 			"101"

>sm_cvar sv_maxcmdrate 			"101"

>sm_cvar cl_cmdrate			"101"

>sm_cvar cl_updaterate 			"101"

>sm_cvar rate				"100000"

>sm_cvar fps_max    "0"

**Step 4:** Change the Launch Parameters.
  * -console -game left4dead -tickrate 100 +log on +map l4d_vs_airport01_greenhouse +exec server +sv_lan 0
  * If you're going to adjust your Tickrate above 100, you will run into Boomer Vomit Range issues. You will need to add   
  ***-frametime 0.037 -frametime_override 0.037*** to the launch parameters to resolve this, make sure to place them after the tickrate parameter.

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
>click [here](https://github.com/fbef0102/L4D1-Server4Dead/releases/download/v2.0/Sourcemod_Anti-Cheat.zip) to download package
[Sourcemod Anti-Cheat Wiki home](https://bitbucket.org/anticheat/smac/wiki/Home)
* smac + smac_aimbot + smac_autotrigger + smac_client + smac_commands + smac_eyetest + smac_rcon + smac_speedhack + smac_spinhack + smac_cvars

# Others
* <b>[L4D1-Competitive-Plugins](https://github.com/fbef0102/L4D1-Competitive-Plugins)</b>: Setup your own L4D1 Servers.
* <b>[Rotoblin-AZMod](https://github.com/fbef0102/Rotoblin-AZMod)</b>: A Competitive L4D1 Versus Configuration
* <b>[L4D1_2-Plugins](https://github.com/fbef0102/L4D1_2-Plugins)</b>: L4D1/2 general purpose and freaky-fun plugins.
