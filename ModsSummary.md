## Engine Mods ##
In the beginining I was hopeful of no engine mods and as is often the case, ignorance is bliss. The more I analyze it the more that needs to be done. There are a many behavoirs and functions that will require significant engine changes, often along with model changes. So many in fact that I am getting the red pen out to perhaps cut a few things off.

  * 3rd Person - with the current functionality I can't get the correct 3rd person view in Saeurbraten. Even red eclipse which implements angle and a few other 3rd person settings can't get it working.  **IMPORTANT**
  * Weapons - ignoring the modelling/fx aspects, some changes will be neccesary, the load out of the weapons would be detemined by the mech class **MECH CLASS**
  * Mech Performance and Qualities - see mech class **MECH CLASS**
  * Salvage pickup after death - the goodies may be able to be managed with the current engine **MECH CLASS**
  * Heat - complex see [Heat](Heat.md) - thinking about dropping this for the moment **MECH CLASS**
  * Mech Actions: - Torso rotation is the main new motion to implement **IMPORTANT**
  * Input - A joy stock controller mod does exist, have downloaded and will see if I can adapt it **UPDATE 2010 using JoyToKey to map it - see downloads for s/w and cfg file** **UPDATE - able to fudge this for demo**
  * Physics - Cube does more physics amd collision stuff than MA1 had, inc recoil (customizable) Even 'death from above' could probably be faked with a mellee attack **OK**
  * Use unique config/graphics - uses mek- prefaced config filea and mek_prefaced gui files **OK**_

So for the demo the 2 important things are
  1. 3rd person view
  1. Torso rotation (model and engine)

All the items marked Mech Class are to be left to phase 2

## Mechclass Changes ##

This is for pahse 2