## Factorio Blueprints

This is a repo to save and share the blueprint designs I've created in Factorio.  Feel free to copy and modify the blueprints here as I've been inspired or modified prints I've found as well.  To access the string to copy, click on the title.

--------------------

## [Modular Mall](/modular-mall)

Based on Modular Mall by Rahbek

![Module Mall Book](/blueprint-images/modular-mall-book.png)
![Module Mall Book](/blueprint-images/modular-mall-built.png)

Version 1.2 -
* Fixed train, artillery wagon, weapons & defense modules
* Adjusted tiles for transitions
* Adjusted alarm to 4 items per belt
* Changed module order
* Fixed bots module
* Split artillery and shells from weapons (allows spacing for roboports)
* Added double-interface for KotS-style mall

-------------------

## [Tile Mall](/tile-mall)

Based on Compact Tileable Malls by Dangerpigeon

![Module Mall Book](/blueprint-images/tile-mall-book.png)
![Module Mall Book](/blueprint-images/tile-mall-built.png)

Version 1.0 - 
* Added Gears, Bots & Accumlators, Ammo & Bots, Explosives, Nuclear & Silo, Artillery, Concrete, and Power Armor modules
* Modified Belts & Inserters, Electrics & Circuits, Trains & Oil to red belts, removed unused inserters, adjusted circuit limits
* Added template of tiles and resource input for belt management

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

## [Oil Processing](/oil)

This is an add-on to plug into my standard base design to handle all oil-based products, input belts for necessary resources, output belts and pipes for the main bus.

Version 1.0 - 
* Created four stages of design to allow for a staged setup as research is unlocked.

![Oil Processing](/blueprint-images/oil-processing.png)

--------------------

## [LTN-like Vanilla Provider Limiter](/ltn-vanilla-provider-limiter)

This allows for a LTN-like provider station in Vanilla using the arithmetic combinators.  The station allows for a max of two trains, one actively being loaded, a second in stand-by.  One combinator counts the total ores (or plates) held in the chests and divides the total by the max that the cargo train can hold.  In this case, it's set to 24,000 as this supports a 2x6 train.  The first combinator takes the total of the items in the chests, divides by the total and outputs a signal reflecting the ore (or plate) as a whole number which sends a signal to the station to set the train limit for the station.

The second combinator receives this train limit signal and by multiplying by 1, turns that count into an ore (or plate) output signal that can then be transmitted over the global network (if the big electric poles have red or green wires tied to them all).  This allows for monitoring anywhere in the field that is tied to this network to track how many loads of ore (or plate) are available to pick up to monitor base demand.  I based this on a Nilaus video where he had something similar setup.

![LTN Vanilla Provider Limiter](/blueprint-images/train-count-2.png)

--------------------

## [Holiday Display](/holiday-display)

I've been spending time lately learning more about circuits and came across a way to make a clock.  I used that to make a holiday light and train display!  One combinator handles the clock on signal T, the other outputs the same value, but outputs on Signal S to alternate the light colors.

![Holiday Display](/blueprint-images/holiday-display.png)
