# If you appreciate my work, you can [PayPal Donate](https://paypal.me/Harry0215?locale.x=zh_TW) me.
> Click [HERE](https://github.com/fbef0102/L4D1-Server4Dead/releases) to download package
# Linux Server Files/Windows Server Files
* Main
	* **[SourceMod](https://www.sourcemod.net/downloads.php?branch=1.11)**
		* **v1.11-git6968** by AlliedModders LLC

	* **[MetaMod](https://www.sourcemm.net/downloads.php?branch=1.11)**
		* **v1.11-git1155** by AlliedModders LLC

	* **[stripper](https://www.bailopan.net/stripper/snapshots/1.2/)** - Add, filter and modify map entities
		* **v1.2.2-git141** by BAILOPAN

	* **[l4dtoolz](https://github.com/accelerator74/l4dtoolz/releases)** - Unlock Server Slot Limit
		* **v2.0.1** by ivailosp、Accelerator74

	* **[Tickrate Enabler](https://github.com/accelerator74/Tickrate-Enabler/releases)** - Unlock Tickrate
		* **v1.5** by ProdigySim、Spirit_12、Accelerator74、Forgetest

* Extenstion
	* **[REST in Pawn](https://github.com/ErikMinekus/sm-ripext/releases)** - Provides HTTP and JSON natives for plugins
		* **v1.3.1** by ErikMinekus 

	* **[socket](https://github.com/JoinedSenses/sm-ext-socket/releases)** - Provides networking functionality for SourceMod scripts
		* **v3.0.2** by sfPlayer & JoinedSenses 

	* **[sourcescramble](https://github.com/nosoop/SMExt-SourceScramble/releases)** - Memory patches & allocate memory
		* **v0.7.1.1** by nosoop

	* **[Actions](https://forums.alliedmods.net/showthread.php?t=336374)** - Extension provides a natives to hook action event handlers and create custom actions
		* **v3.8.8** by BHaType

	* **CollisionHooks** - Provides a straightforward and easy way to hook and modify collision rules between entities.
		* **v1.3** by [VoiDeD](https://github.com/voided/CollisionHook)、[Spirit_12](https://github.com/Satanic-Spirit/Collisionhook)、[A1mDev](https://github.com/L4D-Community/Collisionhook)

* Extra File
	* **[GeoLite2-City](https://www.maxmind.com/en/home)** - addons\sourcemod\configs\geoip\GeoLite2-City.mmdb
		* **2024-12-06** by MAXMIND

	* **[GeoLite2-Country](https://www.maxmind.com/en/home)** - addons\sourcemod\configs\geoip\GeoLite2-Country.mmdb
		* **2024-12-06** by MAXMIND

# Server Install
* **Step 1:** A [clean L4D1 Dedicated Server](#how-to-download-l4d1-dedicated-server-files).

* **Step 2:** Choose [Windows Server files](https://github.com/fbef0102/L4D1-Server4Dead/releases/download/v4.0/Windows_Server_files.zip) or [Linux Server files](https://github.com/fbef0102/L4D1-Server4Dead/releases/download/v4.0/Linux_Server_files.zip)(depending on the operating system of your server), and place the files provided in the correct folder.

* **Step 3:** Adjust your **server_rates.cfg** to match your rates accordingly.  
	* For 100 Tickrate, you'd want these settings:
		1. ```cfg/server_rates.cfg```
			```php
			sm_cvar sv_minrate 				"100000" 	// tickrate * 1000
			sm_cvar sv_maxrate 				"100000" 	// tickrate * 1000
			sm_cvar sv_minupdaterate 		"101"	 	// tickrate +1
			sm_cvar sv_maxupdaterate 		"101"		// tickrate +1
			sm_cvar sv_mincmdrate 			"101"		// tickrate +1
			sm_cvar sv_maxcmdrate 			"101"		// tickrate +1
			sm_cvar net_splitpacket_maxrate "50000" 	// (tickrate÷2) * 1000
			sm_cvar fps_max					"0"
			```

* **Step 4:** Change the Launch Parameters.
	```
	-console -game left4dead -tickrate 100 +log on +map l4d_vs_airport01_greenhouse +exec server +sv_lan 0 -maxplayers 31
	```

# How to download L4D1 Dedicated Server files:
**Warning: Don't try to download "Left 4 Dead Dedicated Server" from steam library, it's broken!! Use steamcmd instead.**

* **Step 1:** [Download SteamCMD](https://developer.valvesoftware.com/wiki/SteamCMD#Downloading_SteamCMD).

* **Step 2:** launch steamcmd , steamcmd would automatically download required files .

* **Step 3:** after it says "Loading Steam API...OK.", type
	* ```force_install_dir ./l4d1/```
	* ```login xxxx```
		* xxxx is your steam account number 
		* Enter your steam account password
	* ```app_update 222840 validate```

* **Step 4:** Finish downloading and close steamcmd.
	* ```exit```

* **Step 5 (Linux Only):** Dependencies ([Source](https://linuxgsm.com/servers/l4dserver/))
	* Ubuntu =< 20.04
		```
		sudo dpkg --add-architecture i386; sudo apt update; sudo apt install curl wget file tar bzip2 gzip unzip bsdmainutils python3 util-linux ca-certificates binutils bc jq tmux netcat lib32gcc1 lib32stdc++6 libsdl2-2.0-0:i386 steamcmd
		sudo apt install lib32z1
		```
	* Ubuntu => 20.10
		```
		sudo dpkg --add-architecture i386; sudo apt update; sudo apt install curl wget file tar bzip2 gzip unzip bsdmainutils python3 util-linux ca-certificates binutils bc jq tmux netcat lib32gcc-s1 lib32stdc++6 libsdl2-2.0-0:i386 steamcmd
		sudo apt install lib32z1
		```
	* Debian =< 10
		```
		sudo dpkg --add-architecture i386; sudo apt update; sudo apt install curl wget file tar bzip2 gzip unzip bsdmainutils python3 util-linux ca-certificates binutils bc jq tmux netcat lib32gcc1 lib32stdc++6
		sudo apt-get install zlib1g
		```
	* Debian => 11
		```
		sudo dpkg --add-architecture i386; sudo apt update; sudo apt install curl wget file tar bzip2 gzip unzip bsdmainutils python3 util-linux ca-certificates binutils bc jq tmux netcat lib32gcc-s1 lib32stdc++6
		sudo apt-get install zlib1g
		```
	* CentOS
		```
		yum install epel-release
		yum install curl wget tar bzip2 gzip unzip python3 binutils bc jq tmux glibc.i686 libstdc++ libstdc++.i686
		yum install zlib.i686
		```

# Optional Files
* Extension
	* **[cutlrbtreefix](https://github.com/fdxx/cutlrbtreefix/releases)** - Fixed server crash "CUtlRBTree overflow"
		* **v0.3** by fdxx

	* **[Accelerator](https://forums.alliedmods.net/showthread.php?t=277703)** - Crash Reporting That Doesn't Suck
		* **v2.5.0-cd575aa** by asherkin
		* 🟥 After 2024/5/2 update, broken in Linux system

# Others
* <b>[Rotoblin-AZMod](https://github.com/fbef0102/Rotoblin-AZMod)</b>: A Competitive L4D1 Versus Configuration
* <b>[L4D1_2-Plugins](https://github.com/fbef0102/L4D1_2-Plugins)</b>: L4D1/2 general purpose and freaky-fun plugins.
* <b>[Sourcemod Anti-Cheat-SMAC](https://github.com/fbef0102/SMAC)</b>: Server-side plugin comprised of different modules to help protect your gameserver against cheaters.
* <b>[Little-Anti-Cheat](https://github.com/fbef0102/Little-Anti-Cheat)</b>: Open source anti-cheat for source games, and runs on SourceMod.
* <b>[Game-Private_Plugin](https://github.com/fbef0102/Game-Private_Plugin)</b>: Private Plugin List.
