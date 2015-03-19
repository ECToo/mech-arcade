**Aim:** The aim of the project is to reproduce the destructive joy of Mechassault 1, using the Cube2 engine.

**Background:** Mechassault is a Mech shooter and was a flagship release for the much lauded Xbox Live service. The online play was some of the best. Microsoft did not supported the game well, and the future of the game was always grim. Microsoft have not made it 'backward compatible' to run it on the 360. It is rumored that the only reason the original Xbox servers are ran for so long was to support Halo, when they closed, the game went. The follow up game, Mechassault 2 was generally disappointing but does run on the 360 so has some future.
![http://mechbay.teamxbow.org/images/mecharcade_raven.jpg](http://mechbay.teamxbow.org/images/mecharcade_raven.jpg)

**The Cube2 engine** (see Sauerbraten http://sauerbraten.org ) is a well sorted out, open source, 3D, online, multiplayer, game engine that you can produce cross platform programs for Windows, Linux and the Mac. It uses OpenGL so the 360 is out, unless someone has ported OpenGL to the 360 recently. There are a number of games produced with it including some commercial ones. Perhaps the slickest of the open source games was [Blood Frontier](http://bloodfrontier.com). Blood Frontier unfortunately died last year and eventually was resurrected as [Red Eclipse](http://redeclipse.net). Red Eclipse still has not been officially relased.Please note that while the engine is open source, the content may not be. Incidentlly, you can visit the Sauerbraten page at [Koders ](http://www.koders.com/info.aspx?c=ProjectInfo&pid=NHUUHY8MGCQ9EMAYMHKTPNUA8E) to view the source online.

For the intial part of the project we used the original [Sauerbraten](http://sauerbraten.org), which the intial versions of MekArcade could 'piggy back' on, this proved the expansion pack concept. We later tried Blood Frontier, and it offered lots of goodies that made 'mechifying' the game easy, almost code free.

In late 2010 we commisioned 2 mech models in Quake md3 format from Walter, a 3D artist who who did the Blood ASP for MekTek. His site is http://www.nebulastation.net/ and his artwork is at deviant art - you can see a non textured animation of the first mech http://walter-nest.deviantart.com/#/d2z1px7.

Early 2011 we have started the support site http://mekarcade.com

I am putting up the current mapmodels up at http://teamxbow.org/downloads/MapModels/ These are quake md2/3 set up for the cube engine and are released with open licences.

## Work list from March 2011, with May Update ##
  1. A cockpit as Hudguns for the 1st person view in RE, luckily my first attempt with Sauer was relatively successful. **Update May** - Md3 works OK
  1. Trying to get the 'best' 3rd person view - CD **Hold** until mech done
  1. Getting the first mech models sorted out for RE - CD/walter **CRITICAL**
  1. ?Commission the 2nd as an md5, biped, boned the same as the RE models- CD/walter **Hold**
  1. shrink the textures further (? about 30%) and complete set -CD **Update May** underway
  1. finalize map models set -CD -CD **Update May** underway
  1. finish at least 4 basic maps (mars, snow, lava, grassy) as templates -  - see previous thoughts [DemoMaps](DemoMaps.md) and http://code.google.com/p/mech-arcade/issues/detail?id=16 -CD/Tom **Update May** at least 6 maps for TD and some will be suitable for CTF/Defend the Base
  1. finish at least one SP map -Tom -CD **Update May** 2 at least will be available
  1. play with weapons -Tom -CD **Update May** underway - Hypercanon added, sword half modded, grenades available in loadout, starting a 'missile' weapon based on the rocket
  1. learn about RE servers, set one up. -Su-CD **Update May** Set Up!
**Added since March**
  1. Mech and Tank entities - the md3 work but need some fine tuning. Maybe add animated tank if time
  1. Mapmodels - dropship and falling lamppost added - see problem below
  1. Ephrem is setting up the CVS repositry
  1. Added low light/infrared view
  1. Able to trigger md5 animations OK, failed with md3 ?syntax issues
  1. Using a modded Arena mode have been able to emulate the MA 3 weapons style and game play - this works well.
    * Energy, Projectile, Missile weapon systems
    * A loadout screen lets you pick your weapons (two thirds working)
    * Mitigates the one mech problem a bit
    * No items on maps, can still pick up any salvage
    * Started to try adding health as goodies

**JULY** - working md5 mech model! Hooray!!!!!!!!!!

**AUGUST**
The RE devs have implimented a 'sort of' playerclass (league mutator) which I posted about earlier, I've now had a chance to play with it and have found some great stuff. Based on the weapon the player is given a weight (I think) which determines some additional player specific physics such as:
Speed
Jump height
Size
Color
The amount of spawn health can be set for each class
In addition there are 3 extra variables, Jump jets, burn resistance and bleed out

What if I used the weapon model to give each of these classes a different appearence. The weapons are seperate models joined with a tag,  so scaled up they could form the gun arms and even the torso, hence it may be possible to give different appearences to the different classes. For various reasons you would have to  pair the weapons up and make one mesh for both weapons, so you would have only 4 diferent mechs with each with  unique weapon sets. The 4 sorts I have thought about are:
1. Kitfox type, small with JJ - armed with modded 'stick' grenades
2. medium sniper type with JJ
3. medium, no JJ, more health than 2 and better close up weapons
4 heavy, using rocket and gattling gun. Slow, more health

In the next few weeks we package up what we have for a september test release. I probably wont't be able to get the league mode 'mechified' for that release, but it will use a modded arena mode (mecha) that gives you a weapons load out.