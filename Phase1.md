## Parts of Phase 1 ##
Nov 20th 2009 : Sauerpork is a spinoff using a slightly modified the Sauerbraten Engine. See [Sauerpork](Sauerpork.md)
Sept 2010 - 12 months late but looks like we might have the demo out for this Xmas New Year!
### 1. Tool Chain ###
- 100% done. See [ToolChains](ToolChains.md), models, which were the greatest problem, have been sorted out.
### 2. Configuration and Scripting ###
RE offers many options to configure and script, for example some easy changes to mimic Mech behavoir  eg:
  * kamikaze -  set to 3 makes a mech like explosion
  * maxhealth - Inceased global health to 500 gives a much mech like game play
  * jumpscale - set to zero this stops them jumping around like grasshoppers
  * _Note:_ these are for BF, most are differt from SB
To give a mechassault style third person perspective you can use these commands below. Note that I had to spend a bit of time fiddling to get the aim correct in 3rd person
  * thirdperson 1
  * thirdpersondist 40 Camera distance from the player model,
  * thirdpersonshift 0
  * thirdpersonangle 45
  * -Note: SB does not have these commands. Need to change engine to adjust 3rd person
### 3. Compiling, C and the Engine ###
  * Installed code::blocks and MWGNU compiler **OK**
  * Recompiled engine with minor changes **OK**
  * set up a code/project repository **OK**
  * Status:  Functional
Todo:
  * Explore engine - see [here.](ExploringEngine.md)
  * Define needs - always a bit slippery
  * find C coder
### 4. Maps & Map Tool Chain ###
  * Basic map editing **OK**
  * Status:  Functional
  * -Note: I will never be a map maker. Tom will try.
Todo next:
    * See how to import/export .obj files
    * Gain proficency in map making
    * find map makers - try commisioniing.
### 5. Model & Model Tool Chain ###
GMax to the rescue. I can now
    * now I can work with md2/3/5 files.  Misfit and Milkshape do MD2/3