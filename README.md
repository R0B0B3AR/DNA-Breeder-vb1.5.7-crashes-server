DNA-Breeder-vb1.5.7-crashes-server
==================================

---- Minecraft Crash Report ----
// Don't be sad. I'll do better next time, I promise!

Time: 12/25/14 12:14 PM
Description: Ticking block entity

java.lang.NullPointerException: Ticking block entity
	at com.advGenetics.TileEntity.TileEntityDNABreeder.func_145845_h(TileEntityDNABreeder.java:157)
	at net.minecraft.world.World.func_72939_s(World.java:2477)
	at net.minecraft.world.WorldServer.func_72939_s(WorldServer.java:669)
	at net.minecraft.server.MinecraftServer.func_71190_q(MinecraftServer.java:943)
	at net.minecraft.server.dedicated.DedicatedServer.func_71190_q(DedicatedServer.java:423)
	at net.minecraft.server.MinecraftServer.func_71217_p(MinecraftServer.java:798)
	at net.minecraft.server.MinecraftServer.run(MinecraftServer.java:658)
	at java.lang.Thread.run(Unknown Source)


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Stacktrace:
	at com.advGenetics.TileEntity.TileEntityDNABreeder.func_145845_h(TileEntityDNABreeder.java:157)

-- Block entity being ticked --
Details:
	Name: tileentitydnabreeder // com.advGenetics.TileEntity.TileEntityDNABreeder
	Block type: ID #230 (tile.dnaBreeder // com.advGenetics.Blocks.BlockDNABreeder)
	Block data value: 3 / 0x3 / 0b0011
	Block location: World: (1345,64,1272), Chunk: (at 1,4,8 in 84,79; contains blocks 1344,0,1264 to 1359,255,1279), Region: (2,2; contains chunks 64,64 to 95,95, blocks 1024,0,1024 to 1535,255,1535)
	Actual block type: ID #230 (tile.dnaBreeder // com.advGenetics.Blocks.BlockDNABreeder)
	Actual block data value: 3 / 0x3 / 0b0011
Stacktrace:
	at net.minecraft.world.World.func_72939_s(World.java:2477)
	at net.minecraft.world.WorldServer.func_72939_s(WorldServer.java:669)

-- Affected level --
Details:
	Level name: world
	All players: 2 total; [GCEntityPlayerMP['iszy23223'/58, l='world', x=-4276.21, y=61.00, z=908.61](iszy23223 at -4276.207857737417,61.0,908.612848902449), GCEntityPlayerMP['R0B0B3AR'/144, l='world', x=1290.00, y=65.00, z=1310.75](R0B0B3AR at 1290.004455804222,65.0,1310.7495797625752)]
	Chunk stats: ServerChunkCache: 1257 Drop: 0
	Level seed: -3178379006545247742
	Level generator: ID 04 - BIOMESOP, ver 0. Features enabled: true
	Level generator options: 
	Level spawn location: World: (-970,66,-2806), Chunk: (at 6,4,10 in -61,-176; contains blocks -976,0,-2816 to -961,255,-2801), Region: (-2,-6; contains chunks -64,-192 to -33,-161, blocks -1024,0,-3072 to -513,255,-2561)
	Level time: 9758791 game time, 10011881 day time
	Level dimension: 0
	Level storage version: 0x04ABD - Anvil
	Level weather: Rain time: 7416 (now: true), thunder time: 33594 (now: false)
	Level game mode: Game mode: survival (ID 0). Hardcore: false. Cheats: false
Stacktrace:
	at net.minecraft.server.MinecraftServer.func_71190_q(MinecraftServer.java:943)
	at net.minecraft.server.dedicated.DedicatedServer.func_71190_q(DedicatedServer.java:423)
	at net.minecraft.server.MinecraftServer.func_71217_p(MinecraftServer.java:798)
	at net.minecraft.server.MinecraftServer.run(MinecraftServer.java:658)
	at java.lang.Thread.run(Unknown Source)

-- System Details --
Details:
	Minecraft Version: 1.7.10
	Operating System: Windows 8.1 (amd64) version 6.3
	Java Version: 1.8.0_25, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 4954244384 bytes (4724 MB) / 6039797760 bytes (5760 MB) up to 6039797760 bytes (5760 MB)
	JVM Flags: 2 total; -Xmx6000m -Xms6000m
	AABB Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	IntCache: cache: 0, tcache: 0, allocated: 15, tallocated: 96
	FML: MCP v9.05 FML v7.10.85.1231 Cauldron-MCPC-Plus vgit-Cauldron-MCPC-Plus-1.7.10-1.1231.04.209 (MC: 1.7.10) (API v1.7.10-R0.1-SNAPSHOT) Minecraft Forge 10.13.2.1231 36 mods loaded, 36 mods active
	mcp{9.05} [Minecraft Coder Pack] (minecraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	FML{7.10.85.1231} [Forge Mod Loader] (cauldron.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Forge{10.13.2.1231} [Minecraft Forge] (cauldron.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	CodeChickenCore{1.0.4.29} [CodeChicken Core] (minecraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Micdoodlecore{} [Micdoodle8 Core] (minecraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	IC2{2.2.628-experimental} [IndustrialCraft 2] (Industrial-Craft-2-Mod-Experimental-1.7.10.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	CompactSolars{4.4.37.314} [Compact Solar Arrays] (14129423944_CompactSolars-Addon-1.7.10.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	advancedgenetics{1.5.7} [Advanced Genetics] (advancedgenetics-1.7.10-1.5.7.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	AdvancedMachines{1.1.3} [IC2 Advanced Machines Addon] (AdvancedMachinesAS-1.7.10.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BiblioCraft{1.8.2} [BiblioCraft] (BiblioCraft[v1.8.2][MC1.7.10].jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BiomesOPlenty{2.1.0} [Biomes O' Plenty] (BiomesOPlenty-1.7.10-2.1.0.1004-universal.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BiblioWoodsBoP{1.8} [BiblioWoods Biomes O'Plenty Edition] (BiblioWoods[BiomesOPlenty][v1.8].jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Core{6.2.6} [BuildCraft] (buildcraft-6.2.6.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Transport{6.2.6} [BC Transport] (buildcraft-6.2.6.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Silicon{6.2.6} [BC Silicon] (buildcraft-6.2.6.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Builders{6.2.6} [BC Builders] (buildcraft-6.2.6.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Energy{6.2.6} [BC Energy] (buildcraft-6.2.6.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Factory{6.2.6} [BC Factory] (buildcraft-6.2.6.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	dungeonpack{1.7.10-1.0} [Dungeon Pack] (dungeonpack-1.7.10-1.0.jar.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	eplus{1.7.10-3.0.1} [Enchanting Plus] (EnchantingPlus-1.7.10-3.0.1.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	FoodPlus{3.0rS} [§bFood Plus] (Food-Plus-Mod-1.7.10.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	GalacticraftCore{3.0.6} [Galacticraft Core] (GalacticraftCore-1.7-3.0.6.232.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	GalacticraftMars{3.0.6} [Galacticraft Planets] (Galacticraft-Planets-1.7-3.0.6.232.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	InfernalMobs{1.5.4} [Infernal Mobs] (InfernalMobs-1.7.10.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	IronChest{6.0.62.742} [Iron Chest] (ironchest-1.7.10-6.0.62.742-universal.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Mantle{1.7.10-0.3.1.jenkins180} [Mantle] (Mantle-mc1.7.10-0.3.1.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	millenaire{6.0.0} [MillÃ©naire] (millenaire-6.0.0.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	moreplayermodels{1.7.10b} [MorePlayerModels] (More-Player-Models-2-Mod-1.7.10.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	OreSpawn{1.7.10.20.2} [OreSpawn] (orespawn-1.7.10-20.2.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	TwilightForest{2.3.2} [The Twilight Forest] (twilightforest-1.7.10-2.3.2.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ForgeMultipart{1.1.0.309} [Forge Multipart] (ForgeMultipart-1.7.10-1.1.0.309-universal.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	WR-CBE|Core{1.4.1.9} [WR-CBE Core] (WR-CBE-1.7.10-1.4.1.9-universal.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	WR-CBE|Addons{1.4.1.9} [WR-CBE Addons] (WR-CBE-1.7.10-1.4.1.9-universal.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	WR-CBE|Logic{1.4.1.9} [WR-CBE Logic] (WR-CBE-1.7.10-1.4.1.9-universal.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	McMultipart{1.1.0.309} [Minecraft Multipart Plugin] (ForgeMultipart-1.7.10-1.1.0.309-universal.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ForgeMicroblock{1.1.0.309} [Forge Microblocks] (ForgeMultipart-1.7.10-1.1.0.309-universal.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Mantle Environment: DO NOT REPORT THIS CRASH! Unsupported mods in environment: bukkit
	Profiler Position: N/A (disabled)
	Vec3 Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	Player Count: 2 / 5; [GCEntityPlayerMP['iszy23223'/58, l='world', x=-4276.21, y=61.00, z=908.61](iszy23223 at -4276.207857737417,61.0,908.612848902449), GCEntityPlayerMP['R0B0B3AR'/144, l='world', x=1290.00, y=65.00, z=1310.75](R0B0B3AR at 1290.004455804222,65.0,1310.7495797625752)]
	Is Modded: Definitely; Server brand changed to 'cauldron,craftbukkit,mcpc,fml,forge'
	Type: Dedicated Server (map_server.txt)
