# Skyfactory4-Crash
---- Minecraft Crash Report ----

WARNING: coremods are present:
  CorePlugin (SmoothFont-mc1.12.2-2.1.2.jar)
  BedPatch (bedpatch-2.2-1.12.2.jar)
  TransformerLoader (OpenComputers-MC1.12.2-1.7.5.192.jar)
  ForgelinPlugin (Forgelin-1.8.4.jar)
  MekanismCoremod (Mekanism-1.12.2-9.8.3.390.jar)
  Do not report to Forge! (If you haven't disabled the FoamFix coremod, try disabling it in the config! Note that this bit of text will still appear.) (foamfix-0.10.14-1.12.2.jar)
  SqueezerCore (SqueezerPatch-1.12.2-1.0.0.jar)
  ApotheosisCore (Apotheosis-1.12.2-1.12.5.jar)
  CTMCorePlugin (CTM-MC1.12.2-1.0.2.31.jar)
  BNBGamingCore (BNBGamingCore-1.12.2-0.12.0.jar)
  AstralCore (astralsorcery-1.12.2-1.10.27.jar)
  EnderCorePlugin (EnderCore-1.12.2-0.5.76-core.jar)
  LoadingPlugin (ResourceLoader-MC1.12.1-1.5.3.jar)
  MalisisCorePlugin (malisiscore-1.12.2-6.5.1.jar)
  SurgeLoadingPlugin (Surge-1.12.2-2.0.77.jar)
  CoreMod (Aroma1997Core-1.12.2-2.0.0.2.b167.jar)
Contact their authors BEFORE contacting forge

// Hey, that tickles! Hehehe!

Time: 7/1/22 10:43 PM
Description: Unexpected error

java.lang.NullPointerException: Unexpected error
	at net.minecraft.world.World.func_189509_E(World.java:225)
	at net.minecraft.world.World.func_180495_p(World.java:905)
	at matteroverdrive.blocks.BlockBoundingBox.getPickBlock(BlockBoundingBox.java:78)
	at mcp.mobius.waila.api.impl.DataAccessorCommon.set(DataAccessorCommon.java:61)
	at mcp.mobius.waila.api.impl.DataAccessorCommon.set(DataAccessorCommon.java:44)
	at mcp.mobius.waila.overlay.WailaTickHandler.tickClient(WailaTickHandler.java:76)
	at net.minecraftforge.fml.common.eventhandler.ASMEventHandler_54_WailaTickHandler_tickClient_ClientTickEvent.invoke(.dynamic)
	at net.minecraftforge.fml.common.eventhandler.ASMEventHandler.invoke(ASMEventHandler.java:90)
	at net.minecraftforge.fml.common.eventhandler.EventBus.post(EventBus.java:182)
	at net.minecraftforge.fml.common.FMLCommonHandler.onPreClientTick(FMLCommonHandler.java:344)
	at net.minecraft.client.Minecraft.func_71407_l(Minecraft.java:1708)
	at net.minecraft.client.Minecraft.func_71411_J(Minecraft.java:1098)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:398)
	at net.minecraft.client.main.Main.main(SourceFile:123)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:497)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Thread: Client thread
Stacktrace:
	at net.minecraft.world.World.func_189509_E(World.java:225)
	at net.minecraft.world.World.func_180495_p(World.java:905)
	at matteroverdrive.blocks.BlockBoundingBox.getPickBlock(BlockBoundingBox.java:78)
	at mcp.mobius.waila.api.impl.DataAccessorCommon.set(DataAccessorCommon.java:61)
	at mcp.mobius.waila.api.impl.DataAccessorCommon.set(DataAccessorCommon.java:44)
	at mcp.mobius.waila.overlay.WailaTickHandler.tickClient(WailaTickHandler.java:76)
	at net.minecraftforge.fml.common.eventhandler.ASMEventHandler_54_WailaTickHandler_tickClient_ClientTickEvent.invoke(.dynamic)
	at net.minecraftforge.fml.common.eventhandler.ASMEventHandler.invoke(ASMEventHandler.java:90)
	at net.minecraftforge.fml.common.eventhandler.EventBus.post(EventBus.java:182)
	at net.minecraftforge.fml.common.FMLCommonHandler.onPreClientTick(FMLCommonHandler.java:344)

-- Affected level --
Details:
	Level name: MpServer
	All players: 1 total; [EntityPlayerSP['Luckrust'/169, l='MpServer', x=-0.95, y=62.00, z=-29.54]]
	Chunk stats: MultiplayerChunkCache: 625, 625
	Level seed: 0
	Level generator: ID 10 - topography, ver 0. Features enabled: false
	Level generator options: 
	Level spawn location: World: (2,72,2), Chunk: (at 2,4,2 in 0,0; contains blocks 0,0,0 to 15,255,15), Region: (0,0; contains chunks 0,0 to 31,31, blocks 0,0,0 to 511,255,511)
	Level time: 3589651 game time, 3603478 day time
	Level dimension: 0
	Level storage version: 0x00000 - Unknown?
	Level weather: Rain time: 0 (now: false), thunder time: 0 (now: false)
	Level game mode: Game mode: survival (ID 0). Hardcore: false. Cheats: false
	Forced entities: 156 total; [EntityBat['Bat'/8, l='MpServer', x=15.03, y=63.10, z=-18.61], EntityStatueBat['Statue Bat'/9, l='MpServer', x=15.63, y=63.10, z=-20.19], EntityStatueBat['Statue Bat'/10, l='MpServer', x=14.25, y=63.10, z=-20.53], EntityStatueBat['Statue Bat'/11, l='MpServer', x=15.17, y=63.10, z=-20.64], EntityStatueBat['Statue Bat'/12, l='MpServer', x=14.25, y=63.10, z=-17.52], EntityBat['Bat'/13, l='MpServer', x=14.25, y=63.10, z=-11.42], EntityBat['Bat'/14, l='MpServer', x=14.25, y=63.10, z=-11.25], EntityStatueBat['Statue Bat'/15, l='MpServer', x=14.25, y=63.10, z=-12.48], EntityBat['Bat'/16, l='MpServer', x=14.25, y=63.10, z=-11.50], EntityStatueBat['Statue Bat'/17, l='MpServer', x=14.25, y=63.10, z=-13.46], EntityStatueBat['Statue Bat'/18, l='MpServer', x=15.18, y=63.10, z=-13.45], EntityBat['Bat'/19, l='MpServer', x=14.44, y=63.10, z=-11.25], EntityStatueBat['Statue Bat'/20, l='MpServer', x=14.25, y=63.10, z=-11.25], EntityBat['Bat'/21, l='MpServer', x=14.25, y=63.10, z=-11.25], EntityStatueBat['Statue Bat'/22, l='MpServer', x=14.25, y=63.10, z=-11.25], EntityBat['Bat'/23, l='MpServer', x=14.25, y=63.10, z=-14.55], EntityStatueBat['Statue Bat'/24, l='MpServer', x=14.38, y=63.10, z=-12.38], EntityStatueBat['Statue Bat'/25, l='MpServer', x=14.57, y=63.10, z=-15.35], EntityStatueBat['Statue Bat'/26, l='MpServer', x=14.25, y=63.10, z=-14.51], EntityBat['Bat'/27, l='MpServer', x=14.38, y=63.10, z=-15.20], EntityBat['Bat'/28, l='MpServer', x=14.56, y=63.10, z=-14.44], EntityCow['Cow'/29, l='MpServer', x=31.11, y=65.00, z=-43.93], EntityChicken['Chicken'/30, l='MpServer', x=27.67, y=65.00, z=-41.03], EntityPig['Pig'/31, l='MpServer', x=31.21, y=65.00, z=-41.58], EntityPig['Pig'/32, l='MpServer', x=28.75, y=65.00, z=-36.49], EntityItem['item.item.egg'/33, l='MpServer', x=26.79, y=65.00, z=-41.45], EntityHorse['Horse'/34, l='MpServer', x=30.89, y=65.00, z=-33.42], EntityStatueBat['Statue Bat'/35, l='MpServer', x=19.39, y=63.10, z=-21.56], EntityStatueBat['Statue Bat'/36, l='MpServer', x=26.75, y=63.10, z=-16.43], EntityStatueBat['Statue Bat'/37, l='MpServer', x=26.75, y=63.10, z=-17.46], EntityStatueBat['Statue Bat'/38, l='MpServer', x=17.47, y=63.10, z=-18.57], EntityStatueBat['Statue Bat'/39, l='MpServer', x=20.36, y=63.10, z=-20.59], EntityBat['Bat'/40, l='MpServer', x=24.65, y=63.10, z=-17.58], EntityBat['Bat'/41, l='MpServer', x=19.14, y=63.10, z=-19.52], EntityStatueBat['Statue Bat'/42, l='MpServer', x=22.53, y=63.10, z=-17.62], EntityBat['Bat'/43, l='MpServer', x=23.47, y=63.10, z=-17.25], EntityBat['Bat'/44, l='MpServer', x=18.59, y=63.10, z=-19.61], EntityStatueBat['Statue Bat'/45, l='MpServer', x=24.87, y=63.10, z=-21.59], EntityStatueBat['Statue Bat'/46, l='MpServer', x=20.44, y=63.10, z=-16.47], EntityBat['Bat'/47, l='MpServer', x=24.78, y=63.10, z=-16.74], EntityStatueBat['Statue Bat'/48, l='MpServer', x=18.48, y=63.10, z=-16.43], EntityBat['Bat'/49, l='MpServer', x=26.58, y=63.10, z=-16.81], EntityBat['Bat'/50, l='MpServer', x=16.46, y=63.10, z=-20.54], EntityBat['Bat'/51, l='MpServer', x=26.75, y=63.10, z=-19.45], EntityBat['Bat'/52, l='MpServer', x=24.79, y=63.10, z=-17.84], EntityItem['item.item.arrow'/53, l='MpServer', x=19.94, y=61.88, z=-16.42], EntityBat['Bat'/54, l='MpServer', x=26.75, y=63.10, z=-19.58], EntityItem['item.item.bone'/55, l='MpServer', x=20.47, y=61.88, z=-17.06], EntityItem['item.item.rottenFlesh'/56, l='MpServer', x=19.94, y=61.88, z=-16.41], EntityBat['Bat'/57, l='MpServer', x=25.47, y=63.10, z=-20.47], EntityItem['item.item.string'/58, l='MpServer', x=19.94, y=61.88, z=-16.49], EntityItem['item.item.sulphur'/59, l='MpServer', x=20.48, y=61.88, z=-17.06], EntityItem['item.item.sulphur'/60, l='MpServer', x=20.50, y=61.88, z=-17.06], EntityItem['item.item.sulphur'/61, l='MpServer', x=19.94, y=61.88, z=-16.46], EntityItem['item.item.rottenFlesh'/62, l='MpServer', x=20.48, y=61.94, z=-16.59], EntityItem['item.item.spiderEye'/63, l='MpServer', x=20.54, y=61.88, z=-17.06], EntityItem['item.item.string'/64, l='MpServer', x=20.47, y=61.88, z=-17.06], EntityItem['item.item.bone'/65, l='MpServer', x=20.37, y=61.94, z=-16.36], EntityItem['item.item.matteroverdrive.tritanium_spine'/66, l='MpServer', x=20.52, y=61.88, z=-17.06], EntityItem['item.item.matteroverdrive.rogue_android_part.head'/67, l='MpServer', x=20.47, y=61.88, z=-17.06], EntityItem['item.item.rottenFlesh'/68, l='MpServer', x=20.46, y=61.94, z=-16.20], EntityItem['item.item.sulphur'/69, l='MpServer', x=20.64, y=61.94, z=-16.40], EntityItem['item.item.spiderEye'/70, l='MpServer', x=20.51, y=61.88, z=-17.06], EntityItem['item.item.matteroverdrive.rogue_android_part.legs'/71, l='MpServer', x=20.50, y=61.88, z=-17.06], EntityItem['item.item.matteroverdrive.weapon_module_ricochet'/72, l='MpServer', x=20.46, y=61.88, z=-17.06], EntityItem['item.item.sulphur'/73, l='MpServer', x=20.54, y=61.88, z=-17.06], EntityItem['item.item.string'/74, l='MpServer', x=20.50, y=61.88, z=-17.06], EntityItem['item.item.arrow'/75, l='MpServer', x=20.36, y=61.94, z=-16.40], EntityItem['item.item.bone'/76, l='MpServer', x=19.94, y=61.88, z=-16.54], EntityItem['item.item.matteroverdrive.weapon_module_ricochet'/77, l='MpServer', x=20.62, y=61.94, z=-16.37], EntityItem['item.item.bone'/78, l='MpServer', x=21.06, y=61.88, z=-16.48], EntityItem['item.item.matteroverdrive.rogue_android_part.arms'/79, l='MpServer', x=21.06, y=61.88, z=-16.46], EntityItem['item.item.matteroverdrive.rogue_android_part.chest'/80, l='MpServer', x=21.06, y=61.88, z=-16.52], EntityItem['item.item.matteroverdrive.weapon_module_barrel.block'/81, l='MpServer', x=20.85, y=61.94, z=-16.66], EntityItem['item.item.rottenFlesh'/82, l='MpServer', x=21.06, y=61.88, z=-16.41], EntityItem['item.item.rottenFlesh'/83, l='MpServer', x=20.50, y=61.88, z=-17.06], EntityItem['item.item.sulphur'/84, l='MpServer', x=19.94, y=61.88, z=-16.51], EntityItem['item.item.arrow'/85, l='MpServer', x=20.45, y=61.94, z=-16.32], EntityItem['item.item.matteroverdrive.rogue_android_part.arms'/86, l='MpServer', x=21.06, y=61.88, z=-16.56], EntityItem['item.item.matteroverdrive.rogue_android_part.head'/87, l='MpServer', x=21.06, y=61.88, z=-16.54], EntityItem['item.item.rottenFlesh'/88, l='MpServer', x=19.94, y=61.88, z=-16.46], EntityItem['item.item.sulphur'/89, l='MpServer', x=19.94, y=61.88, z=-16.49], EntityItem['item.item.matteroverdrive.rogue_android_part.chest'/90, l='MpServer', x=20.52, y=61.94, z=-16.45], EntityItem['item.item.skull.skeleton'/91, l='MpServer', x=19.94, y=61.88, z=-16.58], EntityItem['item.item.sulphur'/92, l='MpServer', x=21.06, y=61.88, z=-16.59], EntityXPOrbBig['entity.xp_orb_big.name'/93, l='MpServer', x=19.81, y=61.88, z=-16.49], EntityItem['item.item.headcrumbs.spider'/94, l='MpServer', x=19.94, y=61.88, z=-16.49], EntityStatueBat['Statue Bat'/95, l='MpServer', x=26.75, y=63.10, z=-11.25], EntityBat['Bat'/96, l='MpServer', x=26.75, y=63.10, z=-14.89], EntityBat['Bat'/97, l='MpServer', x=24.51, y=63.10, z=-13.39], EntityBat['Bat'/98, l='MpServer', x=25.54, y=63.10, z=-14.49], EntityStatueBat['Statue Bat'/99, l='MpServer', x=26.55, y=63.10, z=-15.46], EntityBat['Bat'/100, l='MpServer', x=26.75, y=63.10, z=-11.25], EntityStatueBat['Statue Bat'/101, l='MpServer', x=26.75, y=63.10, z=-14.41], EntityBat['Bat'/102, l='MpServer', x=25.86, y=63.10, z=-13.55], EntityStatueBat['Statue Bat'/103, l='MpServer', x=24.47, y=63.10, z=-13.44], EntityStatueBat['Statue Bat'/104, l='MpServer', x=26.75, y=63.10, z=-15.08], EntityBat['Bat'/105, l='MpServer', x=23.64, y=63.10, z=-11.30], EntityStatueBat['Statue Bat'/106, l='MpServer', x=24.50, y=63.10, z=-11.25], EntityStatueBat['Statue Bat'/107, l='MpServer', x=20.54, y=63.10, z=-11.25], EntityBat['Bat'/108, l='MpServer', x=23.31, y=63.10, z=-14.44], EntityBat['Bat'/109, l='MpServer', x=24.46, y=63.10, z=-15.86], EntityBat['Bat'/110, l='MpServer', x=22.61, y=63.10, z=-12.67], EntityBat['Bat'/111, l='MpServer', x=20.51, y=63.10, z=-15.55], EntityStatueBat['Statue Bat'/112, l='MpServer', x=16.64, y=63.10, z=-11.25], EntityStatueBat['Statue Bat'/113, l='MpServer', x=23.68, y=63.10, z=-16.00], EntityStatueBat['Statue Bat'/114, l='MpServer', x=18.67, y=63.10, z=-15.71], EntityStatueBat['Statue Bat'/115, l='MpServer', x=20.51, y=63.10, z=-13.51], EntityBat['Bat'/116, l='MpServer', x=17.40, y=63.10, z=-11.41], EntityBat['Bat'/117, l='MpServer', x=21.36, y=63.10, z=-14.46], EntityBat['Bat'/118, l='MpServer', x=18.27, y=63.10, z=-15.50], EntityStatueBat['Statue Bat'/119, l='MpServer', x=17.41, y=63.10, z=-11.25], EntityBat['Bat'/120, l='MpServer', x=17.36, y=63.10, z=-12.24], EntityBat['Bat'/121, l='MpServer', x=21.61, y=63.10, z=-12.61], EntityStatueBat['Statue Bat'/122, l='MpServer', x=22.44, y=63.10, z=-12.41], EntityStatueBat['Statue Bat'/123, l='MpServer', x=18.45, y=63.10, z=-14.53], EntityBat['Bat'/124, l='MpServer', x=20.47, y=63.10, z=-11.25], EntityBat['Bat'/125, l='MpServer', x=20.07, y=63.10, z=-11.25], EntityBat['Bat'/126, l='MpServer', x=17.49, y=63.10, z=-15.87], EntityBat['Bat'/127, l='MpServer', x=17.47, y=63.10, z=-13.55], EntityBat['Bat'/128, l='MpServer', x=25.44, y=63.10, z=-11.86], EntityBat['Bat'/129, l='MpServer', x=26.75, y=63.10, z=-12.69], EntityBat['Bat'/130, l='MpServer', x=26.75, y=63.10, z=-15.49], EntityBat['Bat'/131, l='MpServer', x=21.60, y=63.10, z=-13.08], EntityBat['Bat'/132, l='MpServer', x=17.75, y=63.10, z=-11.87], EntityStatueBat['Statue Bat'/133, l='MpServer', x=26.75, y=63.10, z=-14.60], EntityStatueBat['Statue Bat'/134, l='MpServer', x=26.58, y=63.10, z=-11.25], EntityBat['Bat'/135, l='MpServer', x=23.42, y=63.10, z=-11.25], EntityStatueBat['Statue Bat'/136, l='MpServer', x=23.14, y=63.10, z=-11.41], EntityItem['item.item.carrots'/137, l='MpServer', x=20.56, y=61.88, z=-15.94], EntityItem['item.item.matteroverdrive.phaser_rifle'/138, l='MpServer', x=20.51, y=61.88, z=-15.94], EntityBat['Bat'/139, l='MpServer', x=22.51, y=63.10, z=-15.49], EntityStatueBat['Statue Bat'/140, l='MpServer', x=21.94, y=63.10, z=-11.60], EntityBat['Bat'/141, l='MpServer', x=23.48, y=63.10, z=-11.56], EntityItem['item.item.string'/142, l='MpServer', x=20.56, y=61.88, z=-15.94], EntityItem['item.item.spiderEye'/143, l='MpServer', x=20.49, y=61.88, z=-15.94], EntityItem['item.item.sulphur'/144, l='MpServer', x=20.60, y=61.88, z=-15.94], EntityBat['Bat'/145, l='MpServer', x=21.03, y=63.10, z=-14.83], EntityItem['item.item.sulphur'/146, l='MpServer', x=20.55, y=61.88, z=-15.94], EntityItem['item.item.matteroverdrive.rogue_android_part.head'/147, l='MpServer', x=20.53, y=61.88, z=-15.94], EntityItem['item.item.bone'/148, l='MpServer', x=20.55, y=61.88, z=-15.94], EntityItem['item.item.matteroverdrive.rogue_android_part.legs'/149, l='MpServer', x=20.54, y=61.88, z=-15.94], EntityHorse['Horse'/151, l='MpServer', x=33.91, y=65.00, z=-35.86], EntityChicken['Chicken'/152, l='MpServer', x=32.14, y=65.00, z=-34.38], EntityPig['Pig'/153, l='MpServer', x=32.17, y=65.00, z=-32.78], EntityChicken['Chicken'/154, l='MpServer', x=32.11, y=65.00, z=-36.23], EntityChicken['Chicken'/155, l='MpServer', x=32.00, y=65.00, z=-36.72], EntityItem['item.item.egg'/156, l='MpServer', x=33.00, y=65.00, z=-33.87], EntityChicken['Chicken'/157, l='MpServer', x=35.39, y=65.00, z=-21.12], EntityChicken['Chicken'/158, l='MpServer', x=34.17, y=65.00, z=-19.64], EntityHorse['Horse'/159, l='MpServer', x=33.74, y=65.00, z=-30.71], EntityItem['item.item.egg'/160, l='MpServer', x=35.62, y=65.00, z=-20.39], EntityHorse['Horse'/161, l='MpServer', x=35.27, y=65.00, z=-31.99], EntityPlayerSP['Luckrust'/169, l='MpServer', x=-0.95, y=62.00, z=-29.54], EntityLatchedRenderer['unknown'/171, l='MpServer', x=8.50, y=65.00, z=8.50], EntityLatchedRenderer['unknown'/172, l='MpServer', x=-0.95, y=62.00, z=-29.54]]
	Retry entities: 2 total; [EntityLatchedRenderer['unknown'/171, l='MpServer', x=8.50, y=65.00, z=8.50], EntityLatchedRenderer['unknown'/172, l='MpServer', x=-0.95, y=62.00, z=-29.54]]
	Server brand: fml,forge
	Server type: Integrated singleplayer server
Stacktrace:
	at net.minecraft.client.multiplayer.WorldClient.func_72914_a(WorldClient.java:420)
	at net.minecraft.client.Minecraft.func_71396_d(Minecraft.java:2741)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:427)
	at net.minecraft.client.main.Main.main(SourceFile:123)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:497)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)

-- System Details --
Details:
	Minecraft Version: 1.12.2
	Operating System: Windows 10 (amd64) version 10.0
	Java Version: 1.8.0_51, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 1293237328 bytes (1233 MB) / 3064463360 bytes (2922 MB) up to 3817865216 bytes (3641 MB)
	JVM Flags: 3 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xmx4096m -Xms256m
	IntCache: cache: 0, tcache: 0, allocated: 0, tallocated: 0
	FML: MCP 9.42 Powered by Forge 14.23.5.2860 217 mods loaded, 217 mods active
	States: 'U' = Unloaded 'L' = Loaded 'C' = Constructed 'H' = Pre-initialized 'I' = Initialized 'J' = Post-initialized 'A' = Available 'D' = Disabled 'E' = Errored

	| State  | ID                       | Version                  | Source                                            | Signature                                |
	|:------ |:------------------------ |:------------------------ |:------------------------------------------------- |:---------------------------------------- |
	| LCHIJA | minecraft                | 1.12.2                   | minecraft.jar                                     | None                                     |
	| LCHIJA | mcp                      | 9.42                     | minecraft.jar                                     | None                                     |
	| LCHIJA | FML                      | 8.0.99.99                | forge-1.12.2-14.23.5.2860.jar                     | e3c3d50c7c986df74c645c0ac54639741c90a557 |
	| LCHIJA | forge                    | 14.23.5.2860             | forge-1.12.2-14.23.5.2860.jar                     | e3c3d50c7c986df74c645c0ac54639741c90a557 |
	| LCHIJA | smoothfontcore           | mc1.12.2-2.1.2           | minecraft.jar                                     | None                                     |
	| LCHIJA | bnbgamingcore            | 0.12.0                   | minecraft.jar                                     | None                                     |
	| LCHIJA | foamfixcore              | 7.7.4                    | minecraft.jar                                     | None                                     |
	| LCHIJA | opencomputers|core       | 1.7.5.192                | minecraft.jar                                     | None                                     |
	| LCHIJA | smoothfont               | mc1.12.2-2.1.2           | SmoothFont-mc1.12.2-2.1.2.jar                     | None                                     |
	| LCHIJA | advancementbook          | 1.0.3                    | Advancement_Book-1.12-1.0.3.jar                   | None                                     |
	| LCHIJA | ctm                      | MC1.12.2-1.0.2.31        | CTM-MC1.12.2-1.0.2.31.jar                         | None                                     |
	| LCHIJA | appliedenergistics2      | rv6-stable-7             | appliedenergistics2-rv6-stable-7.jar              | dfa4d3ac143316c6f32aa1a1beda1e34d42132e5 |
	| LCHIJA | bdlib                    | 1.14.3.12                | bdlib-1.14.3.12-mc1.12.2.jar                      | None                                     |
	| LCHIJA | ae2stuff                 | 0.7.0.4                  | ae2stuff-0.7.0.4-mc1.12.2.jar                     | None                                     |
	| LCHIJA | animalcrops              | 1.12.2-0.2.0             | AnimalCrops-1.12.2-0.2.0.jar                      | None                                     |
	| LCHIJA | mantle                   | 1.12-1.3.3.55            | Mantle-1.12-1.3.3.55.jar                          | None                                     |
	| LCHIJA | inspirations             | 1.12.2-0.2.9             | Inspirations-1.12.2-0.2.9.jar                     | None                                     |
	| LCHIJA | placebo                  | 1.6.0                    | Placebo-1.12.2-1.6.0.jar                          | None                                     |
	| LCHIJA | apotheosis               | 1.12.4                   | Apotheosis-1.12.2-1.12.5.jar                      | None                                     |
	| LCHIJA | baubles                  | 1.5.2                    | Baubles-1.12-1.5.2.jar                            | None                                     |
	| LCHIJA | statues                  | 0.8.9.2                  | statues-1.12.X-0.8.9.2.jar                        | None                                     |
	| LCHIJA | crafttweaker             | 4.1.20                   | CraftTweaker2-1.12-4.1.20.574.jar                 | None                                     |
	| LCHIJA | mtlib                    | 3.0.6                    | MTLib-3.0.6.jar                                   | None                                     |
	| LCHIJA | modtweaker               | 4.0.18                   | modtweaker-4.0.18.jar                             | None                                     |
	| LCHIJA | bookshelf                | 2.3.590                  | Bookshelf-1.12.2-2.3.590.jar                      | d476d1b22b218a10d845928d1665d45fce301b27 |
	| LCHIJA | gamestages               | 2.0.123                  | GameStages-1.12.2-2.0.123.jar                     | d476d1b22b218a10d845928d1665d45fce301b27 |
	| LCHIJA | recipestages             | 1.1.3                    | RecipeStages-1.1.3.jar                            | None                                     |
	| LCHIJA | primitivecrafting        | 1.12.2                   | primitivecrafting-1.12.2-1.4.4.7.jar              | fd21553434f4905f2f73ea7838147ac4ea07bd88 |
	| LCHIJA | jei                      | 4.15.0.295               | jei_1.12.2-4.15.0.295.jar                         | None                                     |
	| LCHIJA | appleskin                | 1.0.14                   | AppleSkin-mc1.12-1.0.14.jar                       | None                                     |
	| LCHIJA | aroma1997core            | 2.0.0.2.b167             | Aroma1997Core-1.12.2-2.0.0.2.b167.jar             | dfbfe4c473253d8c5652417689848f650b2cbe32 |
	| LCHIJA | aromabackup              | 3.0.0.0.b132             | AromaBackup-1.12.2-3.0.0.0.b132.jar               | dfbfe4c473253d8c5652417689848f650b2cbe32 |
	| LCHIJA | aromabackuprecovery      | 3.0.0.0.b132             | AromaBackup-1.12.2-3.0.0.0.b132.jar               | dfbfe4c473253d8c5652417689848f650b2cbe32 |
	| LCHIJA | astralsorcery            | 1.10.27                  | astralsorcery-1.12.2-1.10.27.jar                  | a0f0b759d895c15ceb3e3bcb5f3c2db7c582edf0 |
	| LCHIJA | waila                    | 1.8.26                   | Hwyla-1.8.26-B41_1.12.2.jar                       | None                                     |
	| LCHIJA | bdsandm                  | 0.0.24                   | BarrelsDrumsStorageAndMore-0.0.24.jar             | None                                     |
	| LCHIJA | base                     | 3.13.0                   | base-1.12.2-3.13.0.jar                            | None                                     |
	| LCHIJA | betteradvancements       | 0.1.0.77                 | BetterAdvancements-1.12.2-0.1.0.77.jar            | None                                     |
	| LCHIJA | bibliocraft              | 2.4.5                    | BiblioCraft[v2.4.5][MC1.12.2].jar                 | None                                     |
	| LCHIJA | bnbgaminglib             | 2.17.6                   | BNBGamingLib-1.12.2-2.17.6.jar                    | None                                     |
	| LCHIJA | bonsaitrees              | 1.1.4                    | bonsaitrees-1.1.4-b170.jar                        | None                                     |
	| LCHIJA | bouncy_creepers          | 0.0.4                    | BouncyCreepers-0.0.4.jar                          | None                                     |
	| LCHIJA | buildinggadgets          | 2.8.3                    | BuildingGadgets-2.8.3.jar                         | None                                     |
	| LCHIJA | calmdownzombieguy        | 1.0.0                    | CalmDownZombieGuy-1.12.2-1.0.0.jar                | None                                     |
	| LCHIJA | carryon                  | 1.12.3                   | CarryOn MC1.12.2 v1.12.3.jar                      | 55e88f24d04398481ae6f1ce76f65fd776f14227 |
	| LCHIJA | chisel                   | MC1.12.2-1.0.2.45        | Chisel-MC1.12.2-1.0.2.45.jar                      | None                                     |
	| LCHIJA | twilightforest           | 3.11.1021                | twilightforest-1.12.2-3.11.1021-universal.jar     | None                                     |
	| LCHIJA | tconstruct               | 1.12.2-2.13.0.183        | TConstruct-1.12.2-2.13.0.183.jar                  | None                                     |
	| LCHIJA | ceramics                 | 1.12-1.3.7b              | Ceramics-1.12-1.3.7b.jar                          | None                                     |
	| LCHIJA | chargers                 | 1.2.0.4                  | Chargers-1.12.2-1.2.0.4.jar                       | 58e787c8aafad8b327883f94d4fa544f936d7b01 |
	| LCHIJA | chineseworkshop          | 1.2.6                    | ChineseWorkshop-1.12.2_1.2.6.jar                  | None                                     |
	| LCHIJA | chiselsandbits           | 14.33                    | chiselsandbits-14.33.jar                          | None                                     |
	| LCHIJA | clickmachine             | 1.2.0                    | ClickMachine-1.12.2-1.2.0.jar                     | None                                     |
	| LCHIJA | clienttweaks             | 3.1.11                   | ClientTweaks_1.12.2-3.1.11.jar                    | None                                     |
	| LCHIJA | clumps                   | 3.1.2                    | Clumps-3.1.2.jar                                  | None                                     |
	| LCHIJA | codechickenlib           | 3.2.3.358                | CodeChickenLib-1.12.2-3.2.3.358-universal.jar     | f1850c39b2516232a2108a7bd84d1cb5df93b261 |
	| LCHIJA | fbp                      | 2.4.1                    | FancyBlockParticles-1.12.x-2.4.1.jar              | None                                     |
	| LCHIJA | pdp                      | 1.12.2-1.2.4             | ProportionalDestructionParticles-1.12.2-1.2.4.jar | None                                     |
	| LCHIJA | redstoneflux             | 2.1.1                    | RedstoneFlux-1.12-2.1.1.1-universal.jar           | None                                     |
	| LCHIJA | cofhcore                 | 4.6.6                    | CoFHCore-1.12.2-4.6.6.1-universal.jar             | None                                     |
	| LCHIJA | cofhworld                | 1.4.0                    | CoFHWorld-1.12.2-1.4.0.1-universal.jar            | None                                     |
	| LCHIJA | colouredtooltips         | 1.0.7                    | ColouredTooltips-1.12.2-1.0.7.jar                 | d476d1b22b218a10d845928d1665d45fce301b27 |
	| LCHIJA | cyclopscore              | 1.6.4                    | CyclopsCore-1.12.2-1.6.4.jar                      | bd0353b3e8a2810d60dd584e256e364bc3bedd44 |
	| LCHIJA | commoncapabilities       | 2.4.6                    | CommonCapabilities-1.12.2-2.4.6.jar               | bd0353b3e8a2810d60dd584e256e364bc3bedd44 |
	| LCHIJA | compactmachines3         | 3.0.18                   | compactmachines3-1.12.2-3.0.18-b278.jar           | None                                     |
	| LCHIJA | compactstorage           | 3.1                      | CompactStorage-3.1-12.jar                         | None                                     |
	| LCHIJA | compatched               | 1.6.0                    | ComPatchedStorage-1.12.2-1.6.0.jar                | None                                     |
	| LCHIJA | contenttweaker           | 1.12.2-4.9.1             | ContentTweaker-1.12.2-4.9.1.jar                   | None                                     |
	| LCHIJA | conarm                   | 1.2.5.9                  | conarm-1.12.2-1.2.5.9.jar                         | 2484ef4d131fdc0dca0647aa21b7b944ddb935a1 |
	| LCHIJA | controlling              | 3.0.9                    | Controlling-3.0.9.jar                             | None                                     |
	| LCHIJA | cookingforblockheads     | 6.5.0                    | CookingForBlockheads_1.12.2-6.5.0.jar             | None                                     |
	| LCHIJA | ctgui                    | 1.0.0                    | CraftTweaker2-1.12-4.1.20.574.jar                 | None                                     |
	| LCHIJA | crafttweakerjei          | 2.0.3                    | CraftTweaker2-1.12-4.1.20.574.jar                 | None                                     |
	| LCHIJA | cucumber                 | 1.1.3                    | Cucumber-1.12.2-1.1.3.jar                         | None                                     |
	| LCHIJA | culinaryconstruct        | 1.3.4                    | culinaryconstruct-1.3.4.jar                       | 2484ef4d131fdc0dca0647aa21b7b944ddb935a1 |
	| LCHIJA | custommainmenu           | 2.0.9.1                  | CustomMainMenu-MC1.12.2-2.0.9.1.jar               | None                                     |
	| LCHIJA | fastbench                | 1.7.3                    | FastWorkbench-1.12.2-1.7.3.jar                    | None                                     |
	| LCHIJA | cyclicmagic              | 1.20.3                   | Cyclic-1.12.2-1.20.3.jar                          | 0e5cb559be7d03f3fc18b8cba547d663e25f28af |
	| LCHIJA | darkutils                | 1.8.230                  | DarkUtils-1.12.2-1.8.230.jar                      | d476d1b22b218a10d845928d1665d45fce301b27 |
	| LCHIJA | patchouli                | 1.0-20                   | Patchouli-1.0-20.jar                              | None                                     |
	| LCHIJA | thermalfoundation        | 2.6.7                    | ThermalFoundation-1.12.2-2.6.7.1-universal.jar    | None                                     |
	| LCHIJA | deepmoblearning          | 1.12.2-2.5.4             | deepmoblearning-1.12.2-2.5.4-universal.jar        | None                                     |
	| LCHIJA | journeymap               | 1.12.2-5.7.1             | journeymap-1.12.2-5.7.1.jar                       | None                                     |
	| LCHIJA | defaultoptions           | 9.2.8                    | DefaultOptions_1.12.2-9.2.8.jar                   | None                                     |
	| LCHIJA | dimstages                | 2.0.23                   | DimensionStages-1.12.2-2.0.23.jar                 | d476d1b22b218a10d845928d1665d45fce301b27 |
	| LCHIJA | dragonmurder             | 1.0.1                    | DragonMurder-1.12.2-1.0.1.jar                     | None                                     |
	| LCHIJA | elevatorid               | 1.4.2                    | ElevatorMod-1.12.2-1.4.2.jar                      | None                                     |
	| LCHIJA | enchdesc                 | 1.1.15                   | EnchantmentDescriptions-1.12.2-1.1.15.jar         | d476d1b22b218a10d845928d1665d45fce301b27 |
	| LCHIJA | endercore                | 1.12.2-0.5.76            | EnderCore-1.12.2-0.5.76.jar                       | None                                     |
	| LCHIJA | endercrop                | 1.12.2-1.6.0             | endercrop-1.12.2-1.6.0.jar                        | None                                     |
	| LCHIJA | enderstorage             | 2.4.6.137                | EnderStorage-1.12.2-2.4.6.137-universal.jar       | f1850c39b2516232a2108a7bd84d1cb5df93b261 |
	| LCHIJA | enderutilities           | 0.7.15                   | enderutilities-1.12.2-0.7.15.jar                  | 2b03e1423915a189b8094816baa18f239d576dff |
	| LCHIJA | extendedcrafting         | 1.5.6                    | ExtendedCrafting-1.12.2-1.5.6.jar                 | None                                     |
	| LCHIJA | extracells               | 2.6.5                    | ExtraCells-1.12.2-2.6.5.jar                       | None                                     |
	| LCHIJA | farmingforblockheads     | 3.1.28                   | FarmingForBlockheads_1.12.2-3.1.28.jar            | None                                     |
	| LCHIJA | fastfurnace              | 1.3.1                    | FastFurnace-1.12.2-1.3.1.jar                      | None                                     |
	| LCHIJA | fenceoverhaul            | 1.3.4                    | FenceOverhaul-1.3.4.jar                           | None                                     |
	| LCHIJA | findme                   | 1.1.0                    | findme-1.12.2-1.1.0-8.jar                         | None                                     |
	| LCHIJA | slabmachines             | 1.0.7                    | Slab_Machines-1.0.7.jar                           | None                                     |
	| LCHIJA | mcmultipart              | 2.5.3                    | MCMultiPart-2.5.3.jar                             | None                                     |
	| LCHIJA | mekanism                 | 1.12.2-9.8.3.390         | Mekanism-1.12.2-9.8.3.390.jar                     | None                                     |
	| LCHIJA | sonarcore                | 5.0.19                   | sonarcore-1.12.2-5.0.19-20.jar                    | None                                     |
	| LCHIJA | fluxnetworks             | 4.0.14                   | fluxnetworks-1.12.2-4.0.14-31.jar                 | None                                     |
	| LCHIJA | foamfix                  | 0.10.14-1.12.2           | foamfix-0.10.14-1.12.2.jar                        | None                                     |
	| LCHIJA | forgelin                 | 1.8.4                    | Forgelin-1.8.4.jar                                | None                                     |
	| LCHIJA | forgemultipartcbe        | 2.6.2.83                 | ForgeMultipart-1.12.2-2.6.2.83-universal.jar      | f1850c39b2516232a2108a7bd84d1cb5df93b261 |
	| LCHIJA | microblockcbe            | 2.6.2.83                 | ForgeMultipart-1.12.2-2.6.2.83-universal.jar      | None                                     |
	| LCHIJA | minecraftmultipartcbe    | 2.6.2.83                 | ForgeMultipart-1.12.2-2.6.2.83-universal.jar      | None                                     |
	| LCHIJA | forgivingvoid            | 1.1.0                    | ForgivingVoid_1.12.2-1.1.0.jar                    | None                                     |
	| LCHIJA | guideapi                 | 1.12-2.1.8-63            | Guide-API-1.12-2.1.8-63.jar                       | None                                     |
	| LCHIJA | headcrumbs               | 2.0.4                    | Headcrumbs-1.12.2-2.0.5.17.jar                    | None                                     |
	| LCHIJA | horsepower               | 2.6.4                    | HorsePower-1.12.2-2.6.4.74.jar                    | cd7e958342770a8b17c919055da42c24dfefd879 |
	| LCHIJA | huntingdim               | 1.0.42                   | HuntingDimension-1.12.2-1.0.42.jar                | d476d1b22b218a10d845928d1665d45fce301b27 |
	| LCHIJA | hurtanimationremover     | 1.0.0                    | HurtAnimationRemover-1.12.2-1.0.0.jar             | None                                     |
	| LCHIJA | hydrogel                 | 1.1.0                    | HydroGel-1.12.2-1.1.0.jar                         | None                                     |
	| LCHIJA | ichunutil                | 7.2.0                    | iChunUtil-1.12.2-7.1.4.jar                        | None                                     |
	| LCHIJA | incontrol                | 3.9.16                   | incontrol-1.12-3.9.16.jar                         | None                                     |
	| LCHIJA | teslacorelib             | 1.0.18                   | tesla-core-lib-1.12.2-1.0.18.jar                  | d476d1b22b218a10d845928d1665d45fce301b27 |
	| LCHIJA | industrialforegoing      | 1.12.2-1.12.2            | industrialforegoing-1.12.2-1.12.13-237.jar        | None                                     |
	| LCHIJA | integrateddynamics       | 1.1.6                    | IntegratedDynamics-1.12.2-1.1.6.jar               | bd0353b3e8a2810d60dd584e256e364bc3bedd44 |
	| LCHIJA | integrateddynamicscompat | 1.0.0                    | IntegratedDynamics-1.12.2-1.1.6.jar               | None                                     |
	| LCHIJA | integratedtunnels        | 1.6.11                   | IntegratedTunnels-1.12.2-1.6.11.jar               | bd0353b3e8a2810d60dd584e256e364bc3bedd44 |
	| LCHIJA | integratedtunnelscompat  | 1.0.0                    | IntegratedTunnels-1.12.2-1.6.11.jar               | None                                     |
	| LCHIJA | inventorysorter          | 1.13.3+57                | inventorysorter-1.12.2-1.13.3+57.jar              | None                                     |
	| LCHIJA | ironjetpacks             | 1.1.0                    | IronJetpacks-1.12-2-1.1.0.jar                     | None                                     |
	| LCHIJA | itemstages               | 2.0.51                   | ItemStages-1.12.2-2.0.51.jar                      | d476d1b22b218a10d845928d1665d45fce301b27 |
	| LCHIJA | kleeslabs                | 5.4.12                   | KleeSlabs_1.12.2-5.4.12.jar                       | None                                     |
	| LCHIJA | limitlessstructureblocks | 1.1.0                    | LimitlessStructureBlocks-1.12.2-1.1.0.jar         | None                                     |
	| LCHIJA | loadingscreens           | 0.3.1                    | LoadingScreens-1.12.2-0.3.1.jar                   | None                                     |
	| LCHIJA | lostcities               | 2.0.22                   | lostcities-1.12-2.0.22.jar                        | None                                     |
	| LCHIJA | malisiscore              | 1.12.2-6.5.1-SNAPSHOT    | malisiscore-1.12.2-6.5.1.jar                      | None                                     |
	| LCHIJA | malisisdoors             | 1.12.2-7.3.0             | malisisdoors-1.12.2-7.3.0.jar                     | None                                     |
	| LCHIJA | mcjtylib_ng              | 3.5.4                    | mcjtylib-1.12-3.5.4.jar                           | None                                     |
	| LCHIJA | mekanismgenerators       | 1.12.2-9.8.3.390         | MekanismGenerators-1.12.2-9.8.3.390.jar           | None                                     |
	| LCHIJA | mercurius                | 1.0.6                    | Mercurius-1.12.2.jar                              | None                                     |
	| LCHIJA | mob_grinding_utils       | 0.3.13                   | MobGrindingUtils-0.3.13.jar                       | None                                     |
	| LCHIJA | mobstages                | 2.0.13                   | MobStages-1.12.2-2.0.13.jar                       | d476d1b22b218a10d845928d1665d45fce301b27 |
	| LCHIJA | morecauldrons            | 1.4.6                    | More-Cauldrons-1.4.6.jar                          | None                                     |
	| LCHIJA | morebuckets              | 1.0.4                    | MoreBuckets-1.12.2-1.0.4.jar                      | None                                     |
	| LCHIJA | moreoverlays             | 1.15.1                   | moreoverlays-1.15.1-mc1.12.2.jar                  | None                                     |
	| LCHIJA | morpheus                 | 1.12.2-3.5.106           | Morpheus-1.12.2-3.5.106.jar                       | None                                     |
	| LCHIJA | mousetweaks              | 2.10                     | MouseTweaks-2.10-mc1.12.2.jar                     | None                                     |
	| LCHIJA | mputils                  | 1.5.6                    | MPUtils-1.12.2-1.5.7.jar                          | None                                     |
	| LCHIJA | mpbasic                  | 1.4.7                    | mpbasic-1.12.2-1.4.11.jar                         | None                                     |
	| LCHIJA | mystcraft                | 0.13.7.06                | mystcraft-1.12.2-0.13.7.06.jar                    | None                                     |
	| LCHIJA | mysticalagriculture      | 1.7.5                    | MysticalAgriculture-1.12.2-1.7.5.jar              | None                                     |
	| LCHIJA | mysticalagradditions     | 1.3.2                    | MysticalAgradditions-1.12.2-1.3.2.jar             | None                                     |
	| LCHIJA | neat                     | 1.4-17                   | Neat 1.4-17.jar                                   | None                                     |
	| LCHIJA | nuclearcraft             | 2.18u                    | NuclearCraft-2.18u-1.12.2.jar                     | None                                     |
	| LCHIJA | opencomputers            | 1.7.5.192                | OpenComputers-MC1.12.2-1.7.5.192.jar              | None                                     |
	| LCHIJA | xnet                     | 1.8.2                    | xnet-1.12-1.8.2.jar                               | None                                     |
	| LCHIJA | ocxnetdriver             | 1.0.3                    | ocxnetdriver-1.0.3-b17.jar                        | None                                     |
	| LCHIJA | ogdragon                 | 0.1.4                    | ogdragon-1.12.2-0.1.4.jar                         | None                                     |
	| LCHIJA | oreexcavation            | 1.4.150                  | OreExcavation-1.4.150.jar                         | None                                     |
	| LCHIJA | prestige                 | 1.1.58                   | Prestige-1.12.2-1.1.58.jar                        | d476d1b22b218a10d845928d1665d45fce301b27 |
	| LCHIJA | parabox                  | 2.0.0                    | Parabox-1.12.2-2.0.0.jar                          | None                                     |
	| LCHIJA | pickletweaks             | 2.1.3                    | PickleTweaks-1.12.2-2.1.3.jar                     | None                                     |
	| LCHIJA | planefix                 | 1.0.0                    | PlaneFix-1.12.2-1.0.0.jar                         | None                                     |
	| LCHIJA | portalgun                | 7.1.0                    | PortalGun-1.12.2-7.1.0.jar                        | 4db5c2bd1b556f252a5b8b54b256d381b2a0a6b8 |
	| LCHIJA | practicallogistics2      | 3.0.8                    | practicallogistics2-1.12.2-3.0.8-11.jar           | None                                     |
	| LCHIJA | projecte                 | 1.12.2-PE1.4.1           | ProjectE-1.12.2-PE1.4.1.jar                       | None                                     |
	| LCHIJA | rangedpumps              | 0.5                      | rangedpumps-0.5.jar                               | None                                     |
	| LCHIJA | realfilingcabinet        | 0.2.0.21                 | realfilingcabinet-1.12-0.2.0.21.jar               | None                                     |
	| LCHIJA | resourcehogs             | 1.0.14                   | ResourceHogs-1.12.2-1.0.14.jar                    | None                                     |
	| LCHIJA | resourceloader           | 1.5.3                    | ResourceLoader-MC1.12.1-1.5.3.jar                 | d72e0dd57935b3e9476212aea0c0df352dd76291 |
	| LCHIJA | rftoolspower             | 1.2.0                    | rftoolspower-1.12-1.2.0.jar                       | None                                     |
	| LCHIJA | rustic                   | 1.1.4                    | rustic-1.1.4.jar                                  | None                                     |
	| LCHIJA | valkyrielib              | 1.12.2-2.0.20.1          | valkyrielib-1.12.2-2.0.20.1.jar                   | None                                     |
	| LCHIJA | simplegenerators         | 1.12.2-2.0.20.2          | simplegenerators-1.12.2-2.0.20.2.jar              | None                                     |
	| LCHIJA | storagenetwork           | 1.7.10                   | SimpleStorageNetwork-1.12.2-1.7.10.jar            | None                                     |
	| LCHIJA | simpletomb               | 1.12.2-1.0.0             | simpletomb-1.12.2-1.0.0.jar                       | 0e5cb559be7d03f3fc18b8cba547d663e25f28af |
	| LCHIJA | skybonsais               | 1.0.1                    | SkyBonsais-1.0.1.jar                              | None                                     |
	| LCHIJA | skygrid                  | 1.1.7                    | SkyGrid-1.1.7.jar                                 | None                                     |
	| LCHIJA | slimyboyos               | 1.0.0                    | SlimyBoyos-1.0.0.jar                              | None                                     |
	| LCHIJA | snad                     | 1.12.1-1.7.09.16a        | Snad-1.12.1-1.7.09.16a.jar                        | None                                     |
	| LCHIJA | sqpatch                  | 1.0.0                    | SqueezerPatch-1.12.2-1.0.0.jar                    | None                                     |
	| LCHIJA | stg                      | 1.12.2-1.2.3             | stg-1.12.2-1.2.3.jar                              | None                                     |
	| LCHIJA | sasit                    | 1.1.30                   | StuffASockInIt-1.12.2-1.1.30.jar                  | None                                     |
	| LCHIJA | supersoundmuffler        | 1.0.2.10                 | supersoundmuffler-revived_1.12.2_1.0.2.10.jar     | None                                     |
	| LCHIJA | surge                    | 2.0.77                   | Surge-1.12.2-2.0.77.jar                           | d476d1b22b218a10d845928d1665d45fce301b27 |
	| LCHIJA | sync                     | 7.1.0                    | Sync-1.12.2-7.1.0.jar                             | 4db5c2bd1b556f252a5b8b54b256d381b2a0a6b8 |
	| LCHIJA | tallgates                | 1.0.0                    | TallGates-1.12.2-1.0.0.1.jar                      | None                                     |
	| LCHIJA | telepastries             | 0.3.4                    | TelePastries-0.3.4.jar                            | None                                     |
	| LCHIJA | thermaldynamics          | 2.5.6                    | ThermalDynamics-1.12.2-2.5.6.1-universal.jar      | None                                     |
	| LCHIJA | thermalinnovation        | 0.3.6                    | ThermalInnovation-1.12.2-0.3.6.1-universal.jar    | None                                     |
	| LCHIJA | tcomplement              | 1.12.2-0.4.3             | TinkersComplement-1.12.2-0.4.3.jar                | None                                     |
	| LCHIJA | tinkertoolleveling       | 1.12.2-1.1.0.DEV.b23e769 | TinkerToolLeveling-1.12.2-1.1.0.jar               | None                                     |
	| LCHIJA | tp                       | 3.2.34                   | tinyprogressions-1.12.2-3.3.34-Release.jar        | None                                     |
	| LCHIJA | tipthescales             | 1.0.4                    | TipTheScales-1.12.2-1.0.4.jar                     | None                                     |
	| LCHIJA | toastcontrol             | 1.8.1                    | Toast Control-1.12.2-1.8.1.jar                    | None                                     |
	| LCHIJA | togetherforever          | 1.0.2                    | togetherforever-1.12.2-1.0.12-22.jar              | None                                     |
	| LCHIJA | worldbook                | 1.0.0                    | WorldBook-1.0.0.jar                               | None                                     |
	| LCHIJA | topography               | 1.14.2                   | Topography-1.12.2-1.14.2.jar                      | None                                     |
	| LCHIJA | torchmaster              | 1.8.5.0                  | torchmaster_1.12.2-1.8.5.0.jar                    | None                                     |
	| LCHIJA | translocators            | 2.5.2.81                 | Translocators-1.12.2-2.5.2.81-universal.jar       | f1850c39b2516232a2108a7bd84d1cb5df93b261 |
	| LCHIJA | treegrowingsimulator     | 0.0.4                    | TreeGrowingSimulator2017-1.0.1.jar                | None                                     |
	| LCHIJA | triumph                  | 3.19.2                   | Triumph-1.12.2-3.19.2.jar                         | None                                     |
	| LCHIJA | twitchcrumbs             | 3.0.4                    | Twitchcrumbs_1.12.2-3.0.4.jar                     | None                                     |
	| LCHIJA | uppers                   | 0.0.6                    | Uppers-0.0.6.jar                                  | None                                     |
	| LCHIJA | universalmodifiers       | 1.12.2-1.0.16.1          | valkyrielib-1.12.2-2.0.20.1.jar                   | None                                     |
	| LCHIJA | vc                       | 5.9.16                   | ViesCraft-1.12.2-5.9.16.jar                       | None                                     |
	| LCHIJA | waddles                  | 0.6.0                    | Waddles-1.12.2-0.6.0.jar                          | None                                     |
	| LCHIJA | wailastages              | 2.0.24                   | WailaStages-1.12.2-2.0.24.jar                     | d476d1b22b218a10d845928d1665d45fce301b27 |
	| LCHIJA | walljump                 | 1.3.2                    | walljump-1.12.2-1.3.2.jar                         | None                                     |
	| LCHIJA | wawla                    | 2.6.275                  | Wawla-1.12.2-2.6.275.jar                          | d476d1b22b218a10d845928d1665d45fce301b27 |
	| LCHIJA | weirdinggadget           | 1.0                      | weirdinggadget-1.12.2-2.1.16-universal.jar        | None                                     |
	| LCHIJA | withercrumbs             | @version@                | witherCrumbs-1.12.2-0.11.jar                      | None                                     |
	| LCHIJA | worldutils               | 0.4.2                    | worldutils-1.12.2-0.4.2.jar                       | 2b03e1423915a189b8094816baa18f239d576dff |
	| LCHIJA | xlfoodmod                | 1.12.2-1.9.2             | XL-Food-Mod-1.12.2-1.9.2.jar                      | None                                     |
	| LCHIJA | ynot                     | 0.2.4                    | YNot-0.2.4.jar                                    | None                                     |
	| LCHIJA | yoyos                    | 1.12.2-1.3.3.25          | yoyos_1.12.2-1.3.3.25.jar                         | None                                     |
	| LCHIJA | zenstages                | 0.5.0-null               | zenstages-0.5.0.jar                               | None                                     |
	| LCHIJA | matteroverdrive          | 0.7.0.0                  | MatterOverdrive-1.12.2-0.7.1.0-universal.jar      | None                                     |
	| LCHIJA | reauth                   | 3.6.0                    | reauth-3.6.0.jar                                  | daba0ec4df71b6da841768c49fb873def208a1e3 |
	| LCHIJA | pipemaster               | 1.0.2                    | PipeMaster-1.0.2-b8.jar                           | None                                     |
	| LCHIJA | sky_orchards             | 0.0.12                   | SkyOrchards-0.0.12.jar                            | None                                     |
	| LCHIJA | teslacorelib_registries  | 1.0.18                   | tesla-core-lib-1.12.2-1.0.18.jar                  | None                                     |

	Loaded coremods (and transformers): 
CorePlugin (SmoothFont-mc1.12.2-2.1.2.jar)
  bre.smoothfont.asm.Transformer
BedPatch (bedpatch-2.2-1.12.2.jar)
  com.mordenkainen.bedpatch.BedPatchASM
TransformerLoader (OpenComputers-MC1.12.2-1.7.5.192.jar)
  li.cil.oc.common.asm.ClassTransformer
ForgelinPlugin (Forgelin-1.8.4.jar)
  
MekanismCoremod (Mekanism-1.12.2-9.8.3.390.jar)
  mekanism.coremod.KeybindingMigrationHelper
Do not report to Forge! (If you haven't disabled the FoamFix coremod, try disabling it in the config! Note that this bit of text will still appear.) (foamfix-0.10.14-1.12.2.jar)
  pl.asie.foamfix.coremod.FoamFixTransformer
SqueezerCore (SqueezerPatch-1.12.2-1.0.0.jar)
  shadows.squeezer.Transformer
ApotheosisCore (Apotheosis-1.12.2-1.12.5.jar)
  shadows.ApotheosisTransformer
CTMCorePlugin (CTM-MC1.12.2-1.0.2.31.jar)
  team.chisel.ctm.client.asm.CTMTransformer
BNBGamingCore (BNBGamingCore-1.12.2-0.12.0.jar)
  com.bloodnbonesgaming.bnbgamingcore.core.BNBGamingCoreClassTransformer
AstralCore (astralsorcery-1.12.2-1.10.27.jar)
  
EnderCorePlugin (EnderCore-1.12.2-0.5.76-core.jar)
  com.enderio.core.common.transform.EnderCoreTransformer
  com.enderio.core.common.transform.SimpleMixinPatcher
LoadingPlugin (ResourceLoader-MC1.12.1-1.5.3.jar)
  lumien.resourceloader.asm.ClassTransformer
MalisisCorePlugin (malisiscore-1.12.2-6.5.1.jar)
  
SurgeLoadingPlugin (Surge-1.12.2-2.0.77.jar)
  
CoreMod (Aroma1997Core-1.12.2-2.0.0.2.b167.jar)
  
	GL info: ' Vendor: 'NVIDIA Corporation' Version: '4.6.0 NVIDIA 516.59' Renderer: 'NVIDIA GeForce RTX 3080/PCIe/SSE2'
	AE2 Version: stable rv6-stable-7 for Forge 14.23.5.2768
	Pulsar/inspirations loaded Pulses: 
		- InspirationsShared (Enabled/Forced)
		- InspirationsBuilding (Enabled/Not Forced)
		- InspirationsUtility (Enabled/Not Forced)
		- InspirationsTools (Enabled/Not Forced)
		- InspirationsRecipes (Enabled/Not Forced)
		- InspirationsTweaks (Enabled/Not Forced)
		- InspirationsShared (Enabled/Forced)
		- WailaPlugin (Enabled/Not Forced)
		- TwilightForestPlugin (Enabled/Not Forced)

	Pulsar/tconstruct loaded Pulses: 
		- TinkerCommons (Enabled/Forced)
		- TinkerWorld (Enabled/Not Forced)
		- TinkerTools (Enabled/Not Forced)
		- TinkerHarvestTools (Enabled/Forced)
		- TinkerMeleeWeapons (Enabled/Forced)
		- TinkerRangedWeapons (Enabled/Forced)
		- TinkerModifiers (Enabled/Forced)
		- TinkerSmeltery (Enabled/Not Forced)
		- TinkerGadgets (Enabled/Not Forced)
		- TinkerOredict (Enabled/Forced)
		- TinkerIntegration (Enabled/Forced)
		- TinkerFluids (Enabled/Forced)
		- TinkerMaterials (Enabled/Forced)
		- TinkerModelRegister (Enabled/Forced)
		- chiselIntegration (Enabled/Not Forced)
		- chiselsandbitsIntegration (Enabled/Not Forced)
		- wailaIntegration (Enabled/Not Forced)

	Pulsar/tcomplement loaded Pulses: 
		- ModuleCommons (Enabled/Forced)
		- ModuleMelter (Enabled/Not Forced)
		- ModuleArmor (Enabled/Not Forced)
		- CeramicsPlugin (Enabled/Not Forced)
		- ChiselPlugin (Enabled/Not Forced)
		- ToolLevelingPlugin (Enabled/Not Forced)
		- Oredict (Enabled/Forced)

	List of loaded APIs: 
		* appliedenergistics2|API (rv6) from appliedenergistics2-rv6-stable-7.jar
		* Base|API (1.0.0) from base-1.12.2-3.13.0.jar
		* Baubles|API (1.4.0.2) from Baubles-1.12-1.5.2.jar
		* betteradvancements|API (0.0.11) from Triumph-1.12.2-3.19.2.jar
		* BetterWithModsAPI (Beta 0.6) from AppleSkin-mc1.12-1.0.14.jar
		* Chisel-API (0.0.1) from Chisel-MC1.12.2-1.0.2.45.jar
		* ChiselAPI|Carving (0.0.1) from Chisel-MC1.12.2-1.0.2.45.jar
		* ChiselsAndBitsAPI (14.25.0) from chiselsandbits-14.33.jar
		* cofhapi (2.5.0) from CoFHCore-1.12.2-4.6.6.1-universal.jar
		* commoncapabilities|api (0.0.1) from CommonCapabilities-1.12.2-2.4.6.jar
		* compactstorage (3.1) from CompactStorage-3.1-12.jar
		* ctm-api (0.1.0) from CTM-MC1.12.2-1.0.2.31.jar
		* ctm-api-events (0.1.0) from CTM-MC1.12.2-1.0.2.31.jar
		* ctm-api-models (0.1.0) from CTM-MC1.12.2-1.0.2.31.jar
		* ctm-api-textures (0.1.0) from CTM-MC1.12.2-1.0.2.31.jar
		* ctm-api-utils (0.1.0) from CTM-MC1.12.2-1.0.2.31.jar
		* Culinary Construct API (1) from culinaryconstruct-1.3.4.jar
		* farmingforblockheads|api (1.0) from FarmingForBlockheads_1.12.2-3.1.28.jar
		* Guide-API|API (2.0.0) from Guide-API-1.12-2.1.8-63.jar
		* iChunUtil API (1.2.0) from iChunUtil-1.12.2-7.1.4.jar
		* industrialforegoingapi (5) from industrialforegoing-1.12.2-1.12.13-237.jar
		* integrateddynamics|api (0.2.0) from IntegratedDynamics-1.12.2-1.1.6.jar
		* journeymap|client-api (1.4) from journeymap-1.12.2-5.7.1.jar
		* journeymap|client-api-display (1.4) from journeymap-1.12.2-5.7.1.jar
		* journeymap|client-api-event (1.4) from journeymap-1.12.2-5.7.1.jar
		* journeymap|client-api-model (1.4) from journeymap-1.12.2-5.7.1.jar
		* journeymap|client-api-util (1.4) from journeymap-1.12.2-5.7.1.jar
		* JustEnoughItemsAPI (4.13.0) from jei_1.12.2-4.15.0.295.jar
		* MatterOverdrive|API (0.4.1) from MatterOverdrive-1.12.2-0.7.1.0-universal.jar
		* MekanismAPI|core (9.8.1) from Mekanism-1.12.2-9.8.3.390.jar
		* MekanismAPI|energy (9.8.1) from Mekanism-1.12.2-9.8.3.390.jar
		* MekanismAPI|gas (9.8.1) from Mekanism-1.12.2-9.8.3.390.jar
		* MekanismAPI|infuse (9.8.1) from Mekanism-1.12.2-9.8.3.390.jar
		* MekanismAPI|laser (9.8.1) from Mekanism-1.12.2-9.8.3.390.jar
		* MekanismAPI|transmitter (9.8.1) from Mekanism-1.12.2-9.8.3.390.jar
		* MekanismAPI|util (9.0.0) from Mekanism-1.12.2-9.8.3.390.jar
		* MouseTweaks|API (1.0) from MouseTweaks-2.10-mc1.12.2.jar
		* Mystcraft|API (0.2) from mystcraft-1.12.2-0.13.7.06.jar
		* opencomputersapi|component (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
		* opencomputersapi|core (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
		* opencomputersapi|driver (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
		* opencomputersapi|driver|item (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
		* opencomputersapi|event (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
		* opencomputersapi|filesystem (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
		* opencomputersapi|internal (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
		* opencomputersapi|machine (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
		* opencomputersapi|manual (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
		* opencomputersapi|network (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
		* opencomputersapi|prefab (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
		* PatchouliAPI (6) from Patchouli-1.0-20.jar
		* practicallogistics2-api (3.1) from practicallogistics2-1.12.2-3.0.8-11.jar
		* projecteapi (1.12.2-1.2.0) from ProjectE-1.12.2-PE1.4.1.jar
		* RealFilingCabinetAPI (0) from realfilingcabinet-1.12-0.2.0.21.jar
		* redstonefluxapi (2.1.1) from RedstoneFlux-1.12-2.1.1.1-universal.jar
		* sonarapi (1.0.1) from sonarcore-1.12.2-5.0.19-20.jar
		* togetherforeverapi (1) from togetherforever-1.12.2-1.0.12-22.jar
		* valkyrielib.api (1.12.2-2.0.10a) from valkyrielib-1.12.2-2.0.20.1.jar
		* WailaAPI (1.3) from Hwyla-1.8.26-B41_1.12.2.jar
	AE2 Integration: IC2:OFF, RC:OFF, MFR:OFF, Waila:ON, InvTweaks:OFF, JEI:ON, Mekanism:ON, OpenComputers:ON, THE_ONE_PROBE:OFF, TESLA:OFF, CRAFTTWEAKER:ON
	Launched Version: forge-14.23.5.2860
	LWJGL: 2.9.4
	OpenGL: NVIDIA GeForce RTX 3080/PCIe/SSE2 GL version 4.6.0 NVIDIA 516.59, NVIDIA Corporation
	GL Caps: Using GL 1.3 multitexturing.
Using GL 1.3 texture combiners.
Using framebuffer objects because OpenGL 3.0 is supported and separate blending is supported.
Shaders are available because OpenGL 2.1 is supported.
VBOs are available because OpenGL 1.5 is supported.

	Using VBOs: Yes
	Is Modded: Definitely; Client brand changed to 'fml,forge'
	Type: Client (map_client.txt)
	Resource Packs: 
	Current Language: English (US)
	Profiler Position: N/A (disabled)
	CPU: 20x 12th Gen Intel(R) Core(TM) i7-12700K
