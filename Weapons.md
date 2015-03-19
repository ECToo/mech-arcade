## WEAPONS ##
The weapon types structure is from the game.h file of BF 0.84

**struct weaptypes**

int info, anim, colour, sound, esound, fsound, rsound,
add, max, sub[2](2.md), adelay[2](2.md), rdelay, damage[2](2.md), speed[2](2.md), power, time[2](2.md),
delay, explode[2](2.md), rays[2](2.md), spread[2](2.md), zdiv[2](2.md),
collide[2](2.md), radial[2](2.md);
bool taper[2](2.md), extinguish[2](2.md), burns[2](2.md), follows[2](2.md), reloads, zooms, fullauto[2](2.md),
thrown[2](2.md);
float elasticity[2](2.md), reflectivity[2](2.md), relativity[2](2.md), waterfric[2](2.md), weight[2](2.md),
partsize[2](2.md), partlen[2](2.md),
kickpush[2](2.md), hitpush[2](2.md), maxdist[2](2.md), halo;
const char name, text, item, vwep, proj;

Note: all the weapons consists of the same bunch of data and a model. The model may not contribute to the projectile/fx at all, which makes it easier to adapt to Mechs.I have tabulated it below, hopefully making it a bit more explicable. Ihave also been able to mod and successfully comple  weapons with altered parameters but same model

---
<table width='800' border='1'>
<blockquote><tr>
<blockquote><td width='84'><b>Var Type</b></td>
<td width='106'><b>Weapon Parameter</b></td>
<td width='188'><b>My guess or definite description</b></td>
<td width='166'>Pisto Example</td>
</blockquote></tr>
<tr>
<blockquote><td width='84'><b>int</b></td>
<td width='106'><b> info</b></td>
<td width='188'> </td>
<td width='166'><font face='Courier New' size='2'>WEAP_PISTOL</font></td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>anim</td>
<td width='188'>?how much animation</td>
<td width='166'><font face='Courier New' size='2'>ANIM_PISTOL</font></td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>colour</td>
<td width='188'>?vis fx</td>
<td width='166'><font face='Courier New' size='2'>0x888888</font></td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>sound</td>
<td width='188'>?Fire sound</td>
<td width='166'><font face='Courier New' size='2'>S_PISTOL</font></td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>esound</td>
<td width='188'>?explode/hit snds</td>
<td width='166'><font face='Courier New' size='2'>S_BZAP</font></td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>fsound</td>
<td width='188'>?fire snds</td>
<td width='166'><font face='Courier New' size='2'>S_WHIZZ</font></td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>rsound</td>
<td width='188'>?snds   ?-1 default</td>
<td width='166'>-1 </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>add</td>
<td width='188'>?</td>
<td width='166'>10</td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>max</td>
<td width='188'>?max </td>
<td width='166'>10</td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>sub 2</td>
<td width='188'>?</td>
<td width='166'><font face='Courier New' size='2'>1, 1 </font></td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>adelay 2 </td>
<td width='188'>?</td>
<td width='166'><font face='Courier New' size='2'>100, 200</font></td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>rdelay</td>
<td width='188'>?delay ms</td>
<td width='166'>1000</td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>damage 2</td>
<td width='188'>?amount of damage</td>
<td width='166'><font face='Courier New' size='2'>35, 35</font></td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>speed 2</td>
<td width='188'>Speed of the projectile effect</td>
<td width='166'><font face='Courier New' size='2'>2500, 2500</font></td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>power</td>
<td width='188'>?</td>
<td width='166'>0</td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>time 2</td>
<td width='188'>?</td>
<td width='166'><font face='Courier New' size='2'>2000, 2000 </font>
</td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>delay</td>
<td width='188'>?</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>explode</td>
<td width='188'> </td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>rays</td>
<td width='188'>?vis fx </td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>spread</td>
<td width='188'>?vis fx</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>zdiv</td>
<td width='188'>?vis fx </td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>collide</td>
<td width='188'>?</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>radial</td>
<td width='188'>?</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'><b>bool: </b></td>
<td width='106'>taper</td>
<td width='188'>?</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'>(Yes or No)</td>
<td width='106'>extinguish,</td>
<td width='188'>?</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>burns,</td>
<td width='188'>?vis fx of burn at hit site</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>follows</td>
<td width='188'>?tracking</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>reloads</td>
<td width='188'>?Self reloads</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>zooms</td>
<td width='188'>obv</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>fullauto</td>
<td width='188'>?Self reloads</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>thrown</td>
<td width='188'>Is it thrown?</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'><b>float:</b> </td>
<td width='106'>elasticity</td>
<td width='188'>?</td>
<td width='166'>
,  ,  ,  ,  ,  ;</td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>reflectivity</td>
<td width='188'>?vis fx or richochet</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>relativity</td>
<td width='188'>?</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>waterfric,</td>
<td width='188'>effect of water on speed</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>weight,</td>
<td width='188'>?</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>partsize</td>
<td width='188'> </td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>partlen</td>
<td width='188'> </td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>kickpush</td>
<td width='188'> </td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>hitpush</td>
<td width='188'> </td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>maxdist</td>
<td width='188'>?range</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>halo</td>
<td width='188'>?vis fx</td>
<td width='166'> </td>
</blockquote></tr>
<tr>
<blockquote><td width='84'><b>const char:</b></td>
<td width='106'>name</td>
<td width='188'>?name that appears in game</td>
<td width='166'><font face='Courier New' size='2'>&quot;pistol&quot;</font></td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>text</td>
<td width='188'>?desc</td>
<td width='166'><font face='Courier New' size='2'>&quot;\fa&quot;</font></td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>item</td>
<td width='188'>Path to item (whats that?)</td>
<td width='166'><font face='Courier New' size='2'>
&quot;weapons/pistol/item&quot;</font></td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>vwep</td>
<td width='188'>Path to model used</td>
<td width='166'><font face='Courier New' size='2'>&quot;weapons/pistol/vwep&quot;</font></td>
</blockquote></tr>
<tr>
<blockquote><td width='84'> </td>
<td width='106'>proj</td>
<td width='188'>?</td>
<td width='166'>&quot;&quot;</td>
</blockquote></tr>
</table></blockquote>

---
### Actual Weapons Examples ###
WEAP\_PISTOL, ANIM\_PISTOL, 0x888888, S\_PISTOL, S\_BZAP, S\_WHIZZ, -1,
10, 10, { 1, 1 }, { 100, 200, }, 1000, { 35, 35 }, { 2500, 2500 }, 0, { 2000, 2000 },
0, { 0, 0 }, { 1, 1 }, { 1, 1 }, { 1, 1 },
{ IMPACT\_GEOM|IMPACT\_PLAYER|COLLIDE\_TRACE, IMPACT\_GEOM|IMPACT\_PLAYER|COLLIDE\_TRACE }, { 0, 0 },
{ false, false }, { false, false }, { false, false, }, { true, true }, true, false, { false, true }, { false, false },
{ 0, 0 }, { 0, 0 }, { 0.05f, 0.05f }, { 2, 2 }, { 0, 0 }, { 0.5f, 0.5f }, { 10, 10 },
{ 2, 2 }, { 150, 150 }, { 600, 600 }, 4,
"pistol", "\fa", "weapons/pistol/item", "weapons/pistol/vwep", ""
},
{
WEAP\_SHOTGUN, ANIM\_SHOTGUN, 0xFFFF22, S\_SHOTGUN, S\_BZAP, S\_WHIZZ, S\_RICOCHET,
1, 8, { 1, 2 }, { 500, 750 }, 1000, { 15, 10 }, { 2500, 2000 }, 0, { 1000, 1000 },
0, { 0, 0 }, { 20, 40 }, { 35, 25 }, { 1, 2 },
{ BOUNCE\_GEOM|IMPACT\_PLAYER|COLLIDE\_TRACE|COLLIDE\_OWNER, IMPACT\_GEOM|IMPACT\_PLAYER|COLLIDE\_TRACE }, { 0, 0 },
{ false, false }, { false, false }, { false, false, }, { true, true }, true, false, { false, false }, { false, false },
{ 0.5f, 0.35f }, { 50, 50 }, { 0.05f, 0.05f }, { 2, 2 }, { 25, 25 }, { 0.75f, 0.75f },{ 50, 50 },
{ 15, 15 }, { 20, 40 }, { 80, 200 }, 6,
"shotgun", "\fy", "weapons/shotgun/item", "weapons/shotgun/vwep", ""
},
{
WEAP\_SMG, ANIM\_SMG, 0xFF8822, S\_SMG, S\_BZAP, S\_WHIZZ, S\_RICOCHET,
40, 40, { 1, 5 }, { 75, 300 }, 1500, { 25, 15 }, { 2000, 2000 }, 0, { 1000, 1000 },
0, { 0, 0 }, { 1, 5 }, { 5, 5 }, { 4, 2 },
{ BOUNCE\_GEOM|IMPACT\_PLAYER|COLLIDE\_TRACE|COLLIDE\_OWNER, IMPACT\_GEOM|IMPACT\_PLAYER|COLLIDE\_TRACE }, { 0, 0 },
{ false, false }, { false, false }, { false, false, }, { true, true }, true, false, { true, true }, { false, false },
{ 0.75f, 0.5f }, { 30, 30 }, { 0.05f, 0.05f }, { 2, 2 }, { 0, 0 }, { 0.5f, 0.5f }, { 40, 40 },
{ 0.5f, 3 }, { 100, 120 }, { 200, 300 }, 5,
"smg", "\fo", "weapons/smg/item", "weapons/smg/vwep", ""
},
{
WEAP\_FLAMER, ANIM\_FLAMER, 0xFF2222, S\_FLAMER, S\_BURN, S\_BURNING, -1,
50, 50, { 1, 5 }, { 100, 750 }, 2000, { 6, 2 }, { 150, 200 }, 0, { 400, 600 },
0, { 24, 32}, { 1, 5 }, { 40, 15 }, { 2, 2 },
{ BOUNCE\_GEOM, IMPACT\_GEOM|IMPACT\_PLAYER|COLLIDE\_OWNER }, { 1, 2 },
{ false, false }, { true, true }, { true, true, }, { true, true }, true, false, { true, true }, { false, false },
{ 0.15f, 0.f }, { 45, 0 }, { 0.75f, 0.5f }, { 1, 1 }, { -300, 50 }, { 24, 32 }, { 0, 0 },
{ 0.25f, 1 }, { 20, 40 }, { 50, 100 }, 7,
"flamer", "\fr", "weapons/flamer/item", "weapons/flamer/vwep", ""
},
{
WEAP\_PLASMA, ANIM\_PLASMA, 0x22FFFF, S\_PLASMA, S\_ENERGY, S\_HUM, -1,
20, 20, { 1, 20 }, { 500, 2000 }, 3000, { 20, 25 }, { 1500, 35 }, 0, { 1000, 5000 },
0, { 20, 48 }, { 1, 1 }, { 5, 5 }, { 0, 0 },
{ IMPACT\_GEOM|IMPACT\_PLAYER, IMPACT\_GEOM|COLLIDE\_STICK }, { 2, 2 },
{ true, true }, { true, false }, { false, false, }, { true, true }, true, false, { true, true }, { false, false },
{ 0, 0 }, { 0, 0 }, { 0.125f, 0.175f }, { 1, 1 }, { 0, 0 }, { 18, 42 }, { 0, 0 },
{ 3, 6 }, { 100, 200 }, { 400, 125 }, 5,
"plasma", "\fc", "weapons/plasma/item", "weapons/plasma/vwep", ""
},
{
WEAP\_RIFLE, ANIM\_RIFLE, 0xAA66FF, S\_RIFLE, S\_ENERGY, S\_BZZT, -1,
5, 5, { 1, 1 }, { 500, 1000 }, 2000, { 50, 200 }, { 4000, 40000 }, 0, { 5000, 5000 },
0, { 24, 0 }, { 1, 1 }, { 5, 0 }, { 10, 0 },
{ IMPACT\_GEOM|IMPACT\_PLAYER|COLLIDE\_TRACE, IMPACT\_GEOM|IMPACT\_PLAYER|COLLIDE\_TRACE|COLLIDE\_CONT }, { 0, 0 },
{ false, false }, { false, false }, { false, false, }, { false, false }, true, true, { false, false }, { false, false },
{ 0, 0 }, { 0, 0 }, { 1, 0 }, { 2, 2 }, { 0, 0 }, { 0.65f, 1.5f }, { 1024, 4096 },
{ 5, 0 }, { 200, 600 }, { 0, 0 }, 7,
"rifle", "\fv", "weapons/rifle/item", "weapons/rifle/vwep", ""
},
{
WEAP\_GRENADE, ANIM\_GRENADE, 0x22FF22, S\_GRENADE, S\_EXPLODE, S\_BEEP, S\_TINK,
1, 2, { 1, 1 }, { 1500, 1500 }, 6000, { 300, 300 }, { 225, 225 }, 3000, { 3000, 3000 },
100, { 68, 68 }, { 1, 1 }, { 0, 0 }, { 0, 0 },
{ BOUNCE\_GEOM|BOUNCE\_PLAYER|COLLIDE\_OWNER, IMPACT\_GEOM|COLLIDE\_STICK }, { 0, 0 },
{ false, false }, { false, false }, { true, true, }, { true, true }, false, false, { false, false }, { true, true },
{ 0.5f, 0 }, { 0, 0 }, { 1, 1 }, { 2, 2 }, { 78, 78 }, { 2, 2 }, { 0, 0 },
{ 5, 5 }, { 1000, 750 }, { 300, 300 }, 3,
"grenade", "\fg", "weapons/grenade/item", "weapons/grenade/vwep", "projectiles/grenade"
},
{
WEAP\_INSTA, ANIM\_RIFLE, 0xAA66FF, S\_RIFLE, S\_ENERGY, S\_BZZT, -1,
5, 5, { 1, 1 }, { 500, 1000 }, 2000, { 50, 200 }, { 10000, 40000 }, 0, { 5000, 5000 },
0, { 0, 0 }, { 1, 1 }, { 5, 0 }, { 10, 0 },
{ IMPACT\_GEOM|IMPACT\_PLAYER|COLLIDE\_TRACE, IMPACT\_GEOM|IMPACT\_PLAYER|COLLIDE\_TRACE|COLLIDE\_CONT }, { 0, 0 },
{ false, false }, { false, false }, { false, false, }, { false, false }, true, true, { false, false }, { false, false },
{ 0, 0 }, { 0, 0 }, { 1, 0 }, { 2, 2 }, { 0, 0 }, { 0.65f, 1.5f }, { 1024, 4096 },
{ 5, 0 }, { 300, 600 }, { 0, 0 }, 7,
"rifle", "\fv", "weapons/rifle/item", "weapons/rifle/vwep", ""
},
{
WEAP\_GIBS, ANIM\_GRENADE, 0x660000, S\_SPLOSH, S\_SPLAT, S\_WHIRR, S\_SPLAT,
1, 1, { 1, 1 }, { 500, 500 }, 500, { 25, 25 }, { 500, 500 }, 0, { 1000, 1000 },
100, { 0, 0 }, { 1, 1 }, { 0, 0 }, { 0, 0 },
{ IMPACT\_GEOM|IMPACT\_PLAYER|COLLIDE\_OWNER, IMPACT\_GEOM|IMPACT\_PLAYER|COLLIDE\_OWNER }, { 0, 0 },
{ false, false }, { false, false }, { false, false, }, { true, true }, true, false, { false, false }, { true, true },
{ 0.35f, 0.35f }, { 0, 0 }, { 1, 1 }, { 2, 2 }, { 35, 35 }, { 2, 2 }, { 0, 0 },
{ 5, 5 }, { 100, 100 }, { 500, 500 }, 4,
"gibs", "\fw", "gibc", "gibc", "gibc"



### Hit Effects & Behavoirs ###
{
HIT\_NONE = 0, HIT\_ALT = 1<<0, HIT\_LEGS = 1<<1, HIT\_TORSO = 1<<2, HIT\_HEAD = 1<<3, HIT\_FULL = 1<<4, HIT\_PROJ = 1<<5,
HIT\_EXPLODE = 1<<6, HIT\_BURN = 1<<7, HIT\_MELT = 1<<8, HIT\_DEATH = 1<<9, HIT\_WATER = 1<<10, HIT\_WAVE = 1<<11, HIT\_SPAWN = 1<<12,
HIT\_LOST = 1<<13, HIT\_KILL = 1<<14, HIT\_SFLAGS = HIT\_KILL
};

**hithurts**(x&HIT\_BURN | x&HIT\_EXPLODE | x&HIT\_PROJ | x&HIT\_MELT | x&HIT\_DEATH || x&HIT\_WATER)|
|:---------------|:------------|:------------|:-------------|