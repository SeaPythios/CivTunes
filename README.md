# CivTunes
 Localized music for CivMC

## Installation Instructions:
- Install "MusicTriggers" mod from Modrinth for 1.21.1
- Drag the folder labeled "MusicTriggers" into your \minecraft\config folder
- Enjoy the tunes

## How To Add Your Region:
- In civmc\redirect, add your song with
<song_name> = <youtube link>

- In example\main add song to [songs] following this format:
  ```
	[songs.<songname>] (
		triggers = [ "Zones-zonename" ]
		volume = <"0.1 - 1">
  ```

- Under [triggers] add the location trigger following this format:
  ```
	[[triggers.zones]]

		identifier = <"zone name"> 
			Unique name for the zone
  
		priority = <default: 3300>
			By default the highest priority trigger always
   			wins and will be active. Set this higher to override the global playlist or set localized zones that override larger areas.

		zone_max_x = <"max x coord">
			The X coordinate of the player must be exclusively less than this value
    			for the trigger to activate.

		zone_max_y = <"max x coord">
			The Y coordinate of the player must be exclusively less than this value
    			for the trigger to activate.

		zone_max_z = <"max x coord">
			The Z coordinate of the player must be exclusively less than this value
    			for the trigger to activate.

		zone_min_x = <"min x coord">
			The X coordinate of the player must be exclusively greater than this
    			value for the trigger to activate.

		zone_min_y = <"min x coord">
			The Y coordinate of the player must be exclusively greater than this
    			value for the trigger to activate.

		zone_min_z = <"min x coord">
			The Z coordinate of the player must be exclusively greater than this
    			value for the trigger to activate.
  ```
=======
Please do note this project is heavily WIP at the moment and only includes basic functionality
