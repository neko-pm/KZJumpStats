# KZJumpStats
git repository for KZTimer jumpstats module

## Original plugin from: https://forums.alliedmods.net/showthread.php?t=252392

## Database Config
```CPP
"kzjumpstats"
{
	"driver"	"sqlite"
	"host"		"localhost"
	"database"	"kzjumpstats-sqlite"
	"user"		"root"
	"pass"		""
}
```

## Convars
```CPP
js_dist_min_lj		230.0	//Minimum distance for longjumps to be considered good
js_dist_pro_lj		245.0	//Minimum distance for longjumps to be considered pro
js_dist_leet_lj		250.0	//Minimum distance for longjumps to be considered leet
js_dist_min_wj		200.0	//Minimum distance for weirdjumps to be considered good
js_dist_pro_wj		260.0	//Minimum distance for weirdjumps to be considered pro
js_dist_leet_wj		270.0	//Minimum distance for weirdjumps to be considered leet
js_dist_min_dropbhop	230.0	//Minimum distance for dropbhop to be considered good
js_dist_pro_dropbhop	260.0	//Minimum distance for dropbhop to be considered pro
js_dist_leet_dropbhop	270.0	//Minimum distance for dropbhop to be considered leet
js_dist_min_bhop	240.0	//Minimum distance for bhops to be considered good (client msg)
js_dist_pro_bhop	260.0	//Minimum distance for bhops to be considered pro (client: perfect quake sound,all: green chat message)
js_dist_leet_bhop	270.0	//Minimum distance for bhops to be considered leet (client: godlike quake sound,all: red chat message)
js_dist_min_multibhop	240.0	//Minimum distance for multi bhops to be considered good
js_dist_pro_multibhop	260.0	//Minimum distance for multi bhops to be considered pro
js_dist_leet_multibhop	270.0	//Minimum distance for multi bhops to be considered leet
```

## Client Commands 
```CPP
sm_speed/showkeys	//displays speed, keys and last jump distance (center panel)
sm_sync			//on/off strafe sync in chat
sm_stats		//displays your jumpstats (menu)
sm_sound		//on/off quake sounds
sm_ljblock		//registers a lj block
sm_colorchat		//on/off jumpstats messages of others in chat
sm_jumptop		//top menu (top 20 lj,wj,bhop,multibhop,dropbhop) (menu)
```

## Admin Commands (all require z flag)
```CPP
sm_resetjumpstats		//Resets jump stats
sm_resetallljrecords		//Resets all lj records
sm_resetallljblockrecords	//Resets all lj block records
sm_resetallwjrecords		//Resets all wj records
sm_resetallbhoprecords		//Resets all bhop records
sm_resetalldropbhoprecords	//Resets all drop bjop records
sm_resetallmultibhoprecords	//Resets all multi bhop records
sm_resetljrecord		//Resets lj record for given steamid
sm_resetljblockrecor		//Resets lj block record for given steamid
sm_resetbhoprecord		//Resets bhop record for given steamid
sm_resetdropbhoprecord		//Resets drop bhop record for given steamid
sm_resetwjrecord		//Resets wj record for given steamid
sm_resetmultibhoprecord		//Resets multi bhop record for given steamid
sm_resetplayerjumpstats		//Resets jump stats for given steamid
```