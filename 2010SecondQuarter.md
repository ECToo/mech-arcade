# Using Blood Frontier #

We have been a bit quiet on the development front with Xmas, holidays and birthdays. During this time BF 0.85 has been released (called the beta 2). It seems very stable and includes some nice enhancements.

Broadly the plan for the next 3 months is:

  1. Recompile thwe BF engine to use different configuration files and few cosmetic differneces - same as sauerpig
  1. Otherwise leave the engine alone
  1. Work on maps and mech models - Priority to get Mappers/modellers
  1. Work out how to alter the player model to accomadate mech & vehicle behavoirs
  1. Implement the game pad using joystick to kbd/mouse mapping - see below

# Using the Gamepad #

I managed to get the gamepad to work (buggy) using some old code Sauerbraten code that I found in a mod called SauerMod, which ironically was the parent of BF. However I am not confident I can get it to work in BF so I looked at using 3rd party joystick to kbd/mouse mappers - I tried JoyToKey, which is a piece of Win32 freeware. I plugged in an Xbox 360 controller and it worked! I have got it about 70% right for BF. I have the app and the config files here http://mech-arcade.googlecode.com/files/JoyToKeyboard360.zip. I have seen similar software for MacOS and Linux, so xplatform implementation should be possible.