## Introduction ##

Welcome to the MechArcade wiki. I have done some preliminary work on the project which you can catch up with here in the TeamXbow [Mechbay](http://mechbay.teamxbow.org/cube_to_mech.htm)

## Game Engine Base ##

I have been looking at the 4 most likely cube candidates as the game engine base. Either Blood Frontier http://bloodfrontier.com or Sauerbraten http://sauerbraten.org were the favorites, I did also look at 2 other cousins, the Intensity Engine (= cube + python + javascript = too complex & I couildn't get it to work properly) or Assault Cube, based on cube 1. Another option may be the content free version of Sauerbraten that is being put together. At this point in time it doesn't matter too much as we are not planning to edit the game code much in the first phase. So Blood it is.

## The Plan ##

Only considering the first phase at this stage - read [Phase1](Phase1.md) for progress. In short I want to get a mech model into the  current maps, as a basic a proof of concept. I am reskining the GUI to make it more mech like, and I have to get the 'tool chains' for code, models, maps and graphics working. The single biggest issue so far has been the models - you can read all about my intial misadventures here in the -  [Mechbay](http://mechbay.teamxbow.org/cube_to_mech.htm)

**Note 1:** Main difference(s) between a MA style mech the current player model:

  * the torso rotation and effects of gait
  * the damage fx and gimping
  * targeting fx (nullsig, chaff)
  * invisibility
  * weapon handling
  * heat management - which actually is complex

**Note 2:** The Mech would be a player not a vehicle b/c the cube engine doesn't do vehicles without significant modding the source

