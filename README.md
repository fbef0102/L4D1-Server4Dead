# If you appreciate my work, you can [PayPal Donate](https://paypal.me/Harry0215?locale.x=zh_TW) me.
> Click [HERE](https://github.com/fbef0102/L4D1-Server4Dead/releases) to download package (last edited:2020/10/4)
# Linux Server Files/Windows Server Files
> Recommended system **win 10** for windows and **ubuntu** for linux
* <b>SourceMod 			1.9.0-git6251</b> 	    by AlliedModders LLC
* <b>MetaMod 			1.10.7-git966</b> 	    by AlliedModders LLC
* <b>stripper 			1.2.2-git129</b> 		by BAILOPAN
* <b>l4dtoolz 			1.0.0.9f</b> 		    by ivailosp
* <b>DHooks 			2.2.0-detours14a</b> 	by Dr!fter、Peace-Maker
* <b>Left 4 Downtown 	0.4.7.5(windows)</b>    by Igor "Downtown1" Smirnov 、 Andrew "XBetaAlpha" Burrows 、 AtomicStryker 、 Michael "ProdigySim" Busby 、 Continued by: sentient & raziEiL, <b>(linux)</b> by Spirit_12
* <b>dosprotect 		1.0.0.0-18(windows)</b> by ZombieX2.net、D1maxa <b>(linux broken)</b>
* <b>tickrate 			1.4(windows)</b> 	    by ProdigySim、Spirit_12, <b>(linux)</b> by Harry、Cheng feng.
* <b>GameRules Tools 	1.0</b> 			    by psychonic
* <b>VoiceHook	 		2.0(windows)</b> 	    by Accelerator74, <b>3.0(linux)</b> by Dragokas
* <b>CollisionHooks	 	0.2(linux)</b> 	    	by VoiDeD、Spirit_12, <b>None(windows broken)</b>
* <b>socket				3.0.1</b> 	    		by sfPlayer
* <b>smbz2				0.0.2</b> 	    		by thraaawn, peace-maker

**Step 1:** A [clean L4D1 Dedicated Server](https://github.com/fbef0102/L4D1-Server4Dead/blob/master/README.md#how-to-download-l4d1-dedicated-server-files).

**Step 2:** Choose [Windows Server files](https://github.com/fbef0102/L4D1-Server4Dead/releases/download/v3.0/Windows_Server_files.zip) or [Linux Server files](https://github.com/fbef0102/L4D1-Server4Dead/releases/download/v3.0/Linux_Server_files.zip)(depending on the operating system of your server), and place the files provided in the correct folder.

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
* login anonymous
* force_install_dir ./l4d1/
* app_update 222840 validate

**Step 4:** finish downloading and quit.

# Sourcemod Anti-Cheat
[Sourcemod Anti-Cheat Wiki home](https://bitbucket.org/anticheat/smac/wiki/Home)
* smac + smac_aimbot + smac_autotrigger + smac_client + smac_commands + smac_eyetest + smac_rcon + smac_speedhack + smac_spinhack + smac_cvars

# Others
* <b>[L4D1-Competitive-Plugins](https://github.com/fbef0102/L4D1-Competitive-Plugins)</b>: L4D1 Competitive enhancement, bug/glitch fixes, general purpose and freaky-fun plugins.
* <b>[Rotoblin-AZMod](https://github.com/fbef0102/Rotoblin-AZMod)</b>: A Competitive L4D1 Versus Configuration
* <b>[L4D1_2-Plugins](https://github.com/fbef0102/L4D1_2-Plugins)</b>: L4D1/2 general purpose and freaky-fun plugins.
