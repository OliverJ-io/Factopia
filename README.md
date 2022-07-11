# Game Here
---
    
### Core Concepts
> Sandbox
> Factory
> Open-world

---

### Gameplay
> Explore the world and Automate all the resources

---

### Art
> Isometric view
> Pixel Art

---

### Music
> Plays depending on the time of day
> Plays randomly
> Plays according to the weather
> Plays according to the season
> Plays according to the location

---

### Design
> #### UI
> > Quest System
> > Inventory System
> > Character System
> > Map System
> > Dialog System
> > Research System
> > Currency System
> #### World
> > ##### Terrain
> > > Simple
> > > Biomes
> > > Mountains
> > > Hills
> > > Rivers
> > > Lakes
> > > Seasonal Terrain
> > ##### Resources
> > > Ores
> > > Trees
> > > Water
> > > Food
> > > Animals

---

### Time
> Time in game is measured in ticks. One tick is one second. The game has the following event loops
> > The main event loop is what updates all of your inventory. It executes once every second. Each call to main event loop causes all tiles to run one tick. Mines extract one tick of ore. factories produce one tick of materials or items (assuming enough inputs).
> > The automation event loop. Any automation

### Tiles
> Mines - Extract ore when placed adjacent to an ore deposit.
> > Increasing levels extracts more ore per tick
> > Level 0 - 1 ore per tick
> > Level 1 - 2 ore per tick
> > Level 2 - 4 ore per tick
> Tracks - Connect tiles and move materials and items between them
> ### Ore Deposits
> > Coal
> > Iron
> > Tin
> > Copper
> > Silver
> > Aluminum
> > Gold
> > Uranium
> ### Materials
> > Alloys
> > > Darkened Alloy (Refined Uranium + Energetic Helium)
> > Ingots
> > > Iron Ingot (1 Iron) - Created in the Furnace Factory
> > > Tin Ingot (1 Tin) - Created in the Furnace Factory
> > > Copper Ingot (1 Copper) - Created in the Furnace Factory
> > > Silver Ingot (1 Silver) - Created in the Furnace Factory
> > > Aluminum Ingot (1 Aluminum) - Created in the Furnace Factory
> > > Gold Ingot (1 Gold) - Created in the Furnace Factory
> > > Uranium Ingot (1 Uranium) - Created in the Furnace Factory
> > Refined Materials
> > > Refined Iron (100 Iron Ingots) - Created in the Foundery Factory
> > > Refined Tin (100 Tin Ingots) - Created in the Foundery Factory
> > > Refined Copper (100 Copper Ingots) - Created in the Foundery Factory
> > > Refined Silver (100 Silver Ingots) - Created in the Foundery Factory
> > > Refined Aluminum (100 Aluminum Ingots) - Created in the Foundery Factory
> > > Refined Gold (100 Gold Ingots) - Created in the Foundery Factory
> > > Refined Uranium (100 Uranium Ingots) - Created in the Foundery Factory
> #### Factories - Convert materials into items and assemble items into other items
> > Furnace Factory - Converts raw ore into materials using energy
> > > Requirements: $ to build. $ and upgrade items to upgrade. Consumes energy on each tick to run.
> > Foundry Factory - Converts one or more materials into an item
> > Assembly Factory - Converts two or more items into a new item
> #### Storage - Stores material and items
> > Warehouses
> > Chests
> > Pocket Dimension Storage
> ### Power Plants - Converts materials into energy
> > Windmill - Creates energy from wind
> > > Level 0 - 1 energy per tick
> > > Level 1 - 2 energy per tick
> > > Level 2 - 4 energy per tick
> > Coal Plant - Burns coal to generate energy
> > > Level 0 - 4 energy per tick for 10 coal
> > > Level 1 - 8 energy per tick for 20 coal
> > > Level 2 - 16 energy per tick for 40 coal
> > Nuclear Plant - Splits uranium to generate energy
> > > Level 0 - 16 energy per tick for 1 uranium
> > > Level 1 - 32 energy per tick for 2 uranium
> > > Level 2 - 64 energy per tick for 4 uranium
> > Fusion Reactor - Fuses hydrogen to generate energy
> > > Level 0 - 64 energy per tick for 1 hydrogen
> > > Level 1 - 128 energy per tick for 2 hydrogen
> > > Level 2 - 256 energy per tick for 4 hydrogen
> > Black Hole Reactor - Injects darkened allow into a stablized black hole to release stored energy
> > > Level 0 - 256 energy per tick for 100 darkened alloy
> > > Level 1 - 512 energy per tick for 200 darkened alloy
> > > Level 2 - 1024 energy per tick for 400 darkened alloy
> > Dimentional Rift Reactor - Uses a contained blackholes to stabilize a rift to pull energy from a dimension of pure energy
> > > Level 0 - 1024 energy per tick for 1 contained blackhole
> > > Level 1 - 2048 energy per tick for 2 contained blackholes
> > > Level 2 - 4096 energy per tick for 4 contained blackholes
> > Debug Reactor - Produces near infinte energy
> > > Level 0 - 32736 energy per tick
> ### Item Tree
> > TODO

### Automation
> Automation allows you to write code to take automatic actions based on certain conditions. Using automation a player can
> > Conduct Trade - Buy, Sell, or Trade Items based on certain preconditions such as quantity of inventory or market price
> > Manufacture Items - Manufacture and assemble new items based on certain preconditions such as quantity of inventory or market price
> > Build
