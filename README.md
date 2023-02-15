## Factorio Blueprints

This is a repo to save and share the blueprint designs I've created in Factorio.  Feel free to copy and modify the blueprints here as I've been inspired or modified prints I've found as well.  To access the string to copy, click on the title.

--------------------

## [Tiled Supply Hub](/tiled-supply-hub)

Based on Compact Tileable Malls by Dangerpigeon

![Tiled Supply Hub Book](/blueprint-images/tiled-supply-hub.png)
![Tiled Supply Hub Built](/blueprint-images/tiled-supply-hub-built.png)

Version 1.1 - 
* Renamed to Tiled Supply Hub
* Added crude oil unbarreler in module 5 for flamethrower ammo
* Fixed inserter logic in matteries & ports module
* Adjusted modules that needed processing units to feed from belt
* Added Modules

--------------------

## [Starter Base - 1.2](/starter-base)

Modified from Nilaus' "Jump Start Base".

![Starter Base](/blueprint-images/starter-base.png)

Version 1.2
* Changed layout of turbines, added a chest for additional coal buffer
* Added more steel furnaces
* Added additional iron gear assembling machine for red belts
* Added turrent, grenade, landfill, and rail assembling machines


--------------------

## [Ore Miners](/ore-miners)

![Ore Miners](/blueprint-images/ore-miners-book.png)
![Ore Miners](/blueprint-images/ore-miners-placement.png)

Version 1.2- 
* Added a "triangle" layout for improved output for use with bots that include either effeciency or speed modules for better performance

--------------------

## [Rail Books](/rails)

All based on Brian's Trains 4.19.

Double Narrow Rail Version 1.2 - 
* Added Madzuri circuit to chest and inserters for even loading to ore provider station
* Added 4-Car siding for a smaller siding option
* Adjusted U-turn to be a smaller space as it'll strictly be used for U-turns and not intersections
* Added modified rail crossing
* Added T Intersection to use instead of the U-turn.

![Double Narrow](/blueprint-images/double-narrow.png)

For a standard dimension ribbon world (128).  Trains to travel clockwide.

Ribbon Single Rail Version 1.0 -

* Added straight sections to run along the top and bottom of the world
* Added crossing to create loops to link sides
* Added sidings for loading and unloading
* Added personal siding for player trains
* Added crossing
* Added a 4 station depot to collect resources

![Ribbon Single](/blueprint-images/ribbon-single.png)

--------------------

## [LTN-like Vanilla Provider Limiter](/ltn-vanilla-provider-limiter)

This allows for a LTN-like provider station in Vanilla using the arithmetic combinators.  The station allows for a max of two trains, one actively being loaded, a second in stand-by.  One combinator counts the total ores (or plates) held in the chests and divides the total by the max that the cargo train can hold.  In this case, it's set to 24,000 as this supports a 2x6 train.  The first combinator takes the total of the items in the chests, divides by the total and outputs a signal reflecting the ore (or plate) as a whole number which sends a signal to the station to set the train limit for the station.

The second combinator receives this train limit signal and by multiplying by 1, turns that count into an ore (or plate) output signal that can then be transmitted over the global network (if the big electric poles have red or green wires tied to them all).  This allows for monitoring anywhere in the field that is tied to this network to track how many loads of ore (or plate) are available to pick up to monitor base demand.  I based this on a Nilaus video where he had something similar setup.

![LTN Vanilla Provider Limiter](/blueprint-images/train-count-2.png)

--------------------

## [Map View Power Meter](/map-view-power-meter)

For quite a while I've mostly used the electric network info by clicking on power poles to see the power, or using a basic setup with lights in a spot I'm near frequently (such as near the supply hub/mall).  This had an alarm if the power in the capacity got too low.  It worked well enough, but I wanted to give something new a try.  I had a post saved from u/warbaque for a while to have a vanilla-based view of power levels and steam (https://www.reddit.com/r/factorio/comments/vgt5at/how_to_see_your_nuclear_and_steam_power/).  I hadn't done anything with it, but decided to give it a shot now that I'm getting more comfortable with the logistics network.  I pulled up the percentage bar, made some tweaks to reduce the size some and added lights for a close visual of the power usage.  With this setup, I can see the percentage of power available in the capactors in the map with rail signal states turned on.

![Map View Power Meter](/blueprint-images/map-view-power-meter.png)

--------------------

## [Uranium Processing](/uranium-processing)

This is a design I came up with to process raw uranium into Uranium 238 & 235.  Even without modules, this will process enough U-235 to sustain a nuclear reactor (I typically built a 4 reactor power station and then stack them for space).  The alarms are for early uranium processing.  Once Kovarex processing is unlocked, all but the iron alarm should be removed as when Kovarex processing is added (I uses Nilaus' design), it's best to let the chests fill to capacity to maintain a steady-state.  The steel chests can then be upgraded to either storage or passive provider chests as needed for Kovarex processing.

The uranium fuel cell output and spent fuel cell input is placed to work with this reactor design: https://www.reddit.com/r/factorio/comments/xx23fx/compact_tileable_480mw_nuclear_powerplant/.  Instead of one big reactor, I stack additional as needed.

![Uranium Processing](/blueprint-images/uranium-processing.png)

--------------------

## [Solid Fuel Steam Engine Power Center](/solid-fuel-power-center)

This is a steam engine power center using solid fuel as the fuel source.  With solid fuel and red belts, this can supply 80 steam engines.  There is also a buffer steel chest to hold unto excess solid fuel as backup.  There is also a capacitor that's wired up to the water pumps to shut them down when the capacitor supply is over 25%.  This isn't a design that'll likely be used, but if there is excess oil, then it can use that up.

![Solid Fuel Steam Engine Power Center](/blueprint-images/solid-fuel-power-center.png)

--------------------

## [Modular Mall](/modular-mall)

Based on Modular Mall by Rahbek.  This has been retired as this is now being actively maintained.

Version 1.2 -
* Fixed train, artillery wagon, weapons & defense modules
* Adjusted tiles for transitions
* Adjusted alarm to 4 items per belt
* Changed module order
* Fixed bots module
* Split artillery and shells from weapons (allows spacing for roboports)
* Added double-interface for KotS-style mall

![Modular Mall Book](/blueprint-images/modular-mall-book.png)
![Modular Mall Built](/blueprint-images/modular-mall-built.png)

--------------------

## [Oil Processing](/oil)

This is an add-on to plug into my standard base design to handle all oil-based products, input belts for necessary resources, output belts and pipes for the main bus.  This has been retired as I've switched to a more modular design.

Version 1.0 - 
* Created four stages of design to allow for a staged setup as research is unlocked.

![Oil Processing](/blueprint-images/oil-processing.png)

--------------------

## [Train Counter](/train-counter)

This is a remix of a design I found ##[here](https://forums.factorio.com/viewtopic.php?p=546303#p546303).  I came across this after seeing a post on Reddit where someone added a counter to an intersection to see how many trains pass.  I thought this would be a fun addition to learn more about the logic network in Factorio.  I tried a few designs, but found this one easy to work with.  The changes I made was to simplify the design and make it plug-and-play.  Since I usually have power near, I don't need to worry about that.  With this design, a red wire needs to be connected from the signal to the power pole.  Then a green wire from the pole to the global network (should one be nearby and you'd want to see it globally).  

Version 1.0 -
* Modified design to simply and make it plug-and-play.

![Train Counter](/blueprint-images/train-counter.png)
