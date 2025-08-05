## Factorio Blueprints

This is a repo to save and share the blueprint designs I've created in Factorio.  Feel free to copy and modify the blueprints here as I've been inspired or modified prints I've found as well. To access the string to copy, click on the title. Blueprints are ordered based on upload/modify date, newest at the top.

--------------------

## [Kovarex Modules](/kovarex-modules)

Different kovarex modules based on logistic choice, one for belts and one for bots.

![Kovarex Modules](/blueprint-images/kovarex-modules-1.png)
![Kovarex Modules](/blueprint-images/kovarex-modules-2.png)

Version 1.0 - 
* Created and tested designs.
* 
--------------------

## [Fission Reactor Modules](/fission-reactor-modules)

Fission reactor modules with different power production levels.

![Fission Reactor Modules](/blueprint-images/fission-reactor-modules-1.png)
![Fission Reactor Modules](/blueprint-images/fission-reactor-modules-2.png)
![Fission Reactor Modules](/blueprint-images/fission-reactor-modules-3.png)
![Fission Reactor Modules](/blueprint-images/fission-reactor-modules-4.png)

Version 1.0 - 
* Created and tested designs.

--------------------

## [Steam Engine Modules](/steam-engine-modules)

Steam engine modules with different power production levels.

![Steam Engine Modules](/blueprint-images/steam-engine-modules.png)

Version 1.0 - 
* Created and tested designs.
  
--------------------

## [Intersection Counter](/intersection-counter)

Red input from signal to pole, then green output from pole to network for monitoring.  Returns [item=locomotive] signal with count.  Based on this design: https://forums.factorio.com/viewtopic.php?p=546303#p546303.

![Intersection Counter](/blueprint-images/intersection-counter.png)

Version 1.0 - 
* Created and tested designs.
  
--------------------

## [Armed Turrets](/armed-turrets)

When placed, bots will set the turret and arm them with 30 clips of the chosen ammunition.

![Armed Turrets](/blueprint-images/armed-turrets.png)

Version 1.0 - 
* Created and tested designs.

--------------------

## [Car Fueling Drops](/car-fuelling-drops)

Place to have bots place car and request fuel

![Car Fuelling Drops](/blueprint-images/car-fueling-drops.png)

Version 1.0 - 
* Created and tested design.

--------------------

## [Single SR Latch](/single-sr-latch)

A correct version of the single item SR latch posted by Potential-Carob-3058 at redd.it/1grxsox.  In testing, I found that the logic operations needed to change to operate correctly.

![Single SR Latch](/blueprint-images/single-sr-latch-1.png)
![Single SR Latch](/blueprint-images/single-sr-latch-2.png)

Version 1.0 - 
* Corrected design by Walker/potential-carob 3058 from redd.it/1grxsox.

--------------------

## [1-2 Lane Belt Buffer](/1-2-lane-belt-buffer)

These are in-line buffer/storage of the contents of the built.  Best for single-item belts.  The splitters and inserters are used to pull from the belt into the steel chest, and then back on the belt.  The steel chest can be replace with a logistics chest to feed items into the bot network.  The top design was by me, created for my Warptorio2 runs to have a buffer of items, which is critical for that mod.  The bottom design is from Nilaus and copied to store together.

![1-2 Lane Belt Buffer](/blueprint-images/1-2-lane-belt-buffer.png)

Version 1.1 - 
* Updated 1 lane buffer for optimization

--------------------

## [Radar Station](/radar-station)

This is a design I've saved for sometime (over two years), and one I found on the internet somewhere.  It may have been from the Factorio forums, but I didn't save the source.  It is a stand-alone radar station that doesn't need to be tied into the power network or need a large setup of solar panels and accumlators.  It uses a trick with the decider combinator to toggle the radar on and off to offer continuous scanning.

![Radar Station](/blueprint-images/radar-station.png)

Version 1.0 - 
* Created and tested design

--------------------

## [Simple 1-1 Lane Balancer](/simple-1-1-lane-balancer)

While working on a new kickstart base design, I came across this as a way to balance the sides of a belt in a simpler and a bit more compact way than the standard design.

![Simple 1-1 Lane Balancer](/blueprint-images/simple-1-1-lane-balancer.png)

Version 1.0 - 
* Created and tested design

--------------------

## [9 Digit Display](/9-digit-display)

While the X digit display works well, it is messy.  Watching a Factorio video, I saw a design similar to this, but the video didn't show the combinator settings.  After some trial and error, I figured out how to configure the combinators and set it up with the max digits possible (limited on values in the display panels).  It's a simpler design and easier to adjust.  For a smaller digit display, just removing the most significant digit (left-most) to get the display you want.

![9 Digit Display](/blueprint-images/9-digit-display.png)

Version 1.0 - 
* Created and tested design

--------------------

## [Chasing Lights](/chasing-lights)

This is a design I've been thinking about off and on for some time, but just couldn't think of the way to do it.  While watching a Factorio video, I was inspired by another design to make this work.  The combinator receives the clock value and divides by four (in this design) to create the segments.  Then each light is tied to a value from the dot signal.  This is also parametrized to adjust the timing and number of segments.

![Chasing Lights](/blueprint-images/chasing-lights.gif)

Version 1.0 - 
* Created and tested design

--------------------

## [Universal Train Scheduler](/universal-train-schedule)

With the new interrupt features in Factrio 2.0, it is now possible to setup a universal train schedule. There are two trains, one for cargo and one for fluids. This prevents the wrong train being sent to pickup the wrong request. The train is designed to always go to a refueling depot when not assigned a schedule. Once the depot receives a request through the circuit network, it will send that request to the train. The train will receive the item request and be dispatched to a shipping station supplying the item requested, and once full, route to the receiving station for drop-off.  The green icons in the images below are placeholders for the item request sent through the circuit network. You can see these in the third image, which also shows the naming scheme of the stations.

The stations are also included using the parametrized feature in 2.0. Once placed, the selection GUI will appear to select the item the stations will ship or receive. This choice will also auto-fill both the station and combinator to set the limits for station activation based on how many stacks the station or train can support. The stations also include the new display panels for visual feedback on when the station is active and when a train is being sent to the station.

![Universal Train Scheduler Trains](/blueprint-images/universal-train-scheduler-1.png)
![Universal Train Scheduler Schedule](/blueprint-images/universal-train-scheduler-2.png)
![Universal Train Scheduler Interrupts](/blueprint-images/universal-train-scheduler-3.png)
![Universal Train Scheduler Stations](/blueprint-images/universal-train-scheduler-4.png)

Version 1.1 -
* Updated scheduling and fluid stations

--------------------

## [X Digit Displays](/x-digit-displays)

After seeing a three digit display on [Factorio School](https://www.factorio.school/), I wanted to give this a try. After trying the design I found and that it didn't work right, I made these. I did some searching online to find out how to use division to separate a multi-digit number into individual digits to display. Once I figured out the three digit setup, I expanded to support up to seven digits. The constant combinator will be removed and a red signal will need to be sent into the input of the far right combinator as the input to display.  If the signal coming in is on a green wire, it will need to be converted to red with an arithmetic combintor by either multiplying by 1 or adding 0.

![X Digit Displays](/blueprint-images/x-digit-displays.png)

Version 1.0 - 
* Created and tested design

--------------------

## [Universal Assembler](/universal-assembler)

With the new parametrized feature in 2.0 and seeing content creators make something similar, I created my own. Once placed, set the item to craft and how many to store, and everything else is sent. Can support an item that needs up to 9 ingredients (Spidertron requires 8).

![Universal Assembler Placement](/blueprint-images/universal-assembler-1.png)
![Universal Assembler Set](/blueprint-images/universal-assembler-2.png)

Version 1.1 - 
* Updated logistic connection to assembler

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

## [LTN-like Vanilla Provider Limiter](/ltn-vanilla-provider-limiter)

This allows for a LTN-like provider station in Vanilla using the arithmetic combinators.  The station allows for a max of two trains, one actively being loaded, a second in stand-by.  One combinator counts the total ores (or plates) held in the chests and divides the total by the max that the cargo train can hold.  In this case, it's set to 24,000 as this supports a 2x6 train.  The first combinator takes the total of the items in the chests, divides by the total and outputs a signal reflecting the ore (or plate) as a whole number which sends a signal to the station to set the train limit for the station.

The second combinator receives this train limit signal and by multiplying by 1, turns that count into an ore (or plate) output signal that can then be transmitted over the global network (if the big electric poles have red or green wires tied to them all).  This allows for monitoring anywhere in the field that is tied to this network to track how many loads of ore (or plate) are available to pick up to monitor base demand.  I based this on a Nilaus video where he had something similar setup.

![LTN Vanilla Provider Limiter](/blueprint-images/train-count-2.png)

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

## [Train Counter](/train-counter)

This is a remix of a design I found [here](https://forums.factorio.com/viewtopic.php?p=546303#p546303).  I came across this after seeing a post on Reddit where someone added a counter to an intersection to see how many trains pass.  I thought this would be a fun addition to learn more about the logic network in Factorio.  I tried a few designs, but found this one easy to work with.  The changes I made was to simplify the design and make it plug-and-play.  Since I usually have power near, I don't need to worry about that.  With this design, a red wire needs to be connected from the signal to the power pole.  Then a green wire from the pole to the global network (should one be nearby and you'd want to see it globally).  Once connected, once a train passes the signal to turn it red, then the counter will increment by 1.

Version 1.0 -
* Modified design to simply and make it plug-and-play.

![Train Counter](/blueprint-images/train-counter.png)
