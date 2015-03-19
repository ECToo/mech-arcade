The **basic model** is all that would be needed for our phase 1 testing and further developing a 'reference mech'. Infact we want a model that we can just drop in to the engine NOW, as is. The complex model with all the goodies would be needed for release. Significant change to the engine would be needed to accomadate all the added functionality of the complex model. During Phase 2 we probably actually need to develop 2 reference mechs, a chicken walker and one with a human style gait.
### Basic Model UPDATE August 2010 ###
The model for the demo will need the following basic features:
  * Run animation
  * Walk animation
  * Torso Rotation animation
  * Gimped (damgaged and limping)animation
  * Hit (torso rocks)
  * Destroyed animation - nice big destructive core breach, and maybe some goodies
  * Knocked over
  * Animations are accessed programatically in exactly the same way as the engine currently does, because we want it 'drop in'.
  * Basic parameters like speed, turn speed need to be able to be set programatically
  * Format: MD3 or MD5, suitable for import straight into Blood Frontier/Cube
  * Game Size: 2 - 3 storeys tall
### Complex Model PHASE 2 Second Q 2011 ###
  * Basic Model Animations as described above.
  * Damage Effects
  * Heat Effects - possibly
  * Weapons
  * Jumpjets - for some, eventually
  * Defense - one of Nullsig, Cloak, Antimissile or Shield.
  * ??keep taunt, can a mech taunt? - _'I exhaust my plasma waste in your general direction'_
  * ??Others

---

### We want to Commission a Mech Model ###
Out of my very empty pockets I have found a few credits and even sold my youngest child for a small profit; just so we can ask for Cube Modellers to provide a quote for building us a Mech.

**CUBE MODELLERS SEND US A QUOTE FOR A MECH MODEL - Send to cdxbow@yahoo.com.au**

You can quote for either, though we can't actually handle all the elements in a complex model yet and I would probably have to sell another child to pay for it. That would only leave one for the rest of the project.

To help you along I can send you a number of open source mech models in other formats. I will send them after intial contact. If you simply have advice, I would love to hear it, or recommend an artist, I would be grateful to for that too.

If you don't have a bloody clue what a mech is then look here at the  [The Mechbay](http://mechbay.teamxbow.org/default.htm) You can look at images in the gallery and read articles about Mechs and the game, Mechassault.

**Animations supported by the BF engine: in capital proposed**
  * idle-IDLE
  * forward-WALK F, backward WALK B, left TORSO L, right TORSO R,
  * dead, dying, GIMPED, DEAD
  * pain - _would be damage. Says somewhere these are model specific_ HIT
  * jump - ?Turn this to JUMP JETS
  * impulse forward-RUN F, impulse backward-RUN B, impulse left, impulse right, impulse dash - ???
  * crouch, crawl forward, crawl backward, crawl left, crawl right, - _prone with mov_
  * sink, swim - _jump in the water to see these_
  * mapmodel, trigger on, trigger off, - _?interacting with map effects_
  * edit, lag, switch, ???
  * win, lose
  * pistol, pistol shoot, pistol reload,
  * shotgun, shotgun shoot, shotgun reload,
  * smg, smg shoot, smg reload,
  * grenade, grenade throw, grenade reload, grenade power,
  * flamer, flamer shoot, flamer reload,
  * plasma, plasma shoot, plasma reload,
  * rifle, rifle shoot, rifle reload,
  * vwep, -  _??generic weapon_
  * shield - _?shows you the player has picked up a sheild_
  * powerup - _?shows you the player is powered up_
-**Note: Excluding the weapons I have only seen about a dozen or so of these actually used.**