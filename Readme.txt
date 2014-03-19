Introduction:
This is a Descent 1 Weapons conversion mod.

Release License:
	All changes are under the same license as the underlying Quake 2 Source code license
	Some code courtesy of http://webadvisor.aupr.edu/noc/CodingTutorials.htm

Features:
	9 weapons from descent 1
	1 weapon from descent 2
	Shared energy system for primary weapons like in Descent 1/2
	2 accessories from descent 1/2
	Ability to fly like in Descent

Notes:	
	Only tested in single player mode
	Weapons function like they do in Descent 1/2, but are not balanced for damage/ammo usage

Bugs:
	Flying logic is only partially finished
	Weapon pickups have not been tested, new weapons require updated maps to appear(?)
	Mines cannot detonate on player that spawned them
	Smart missiles do not work properly

Compiling:
* Visual Studio 2008: 
   1)	Open the game.dsp (VC++ 6 Project) and let it convert
   2)	Change the release type to "Release"
   3)	Compile
   4)	dll will be at "..\Releases\gamex86.dll"
   5)	Move dll to <quake 2 root folder>\baseq2 (overwrite the existing one)
   6)	Run

* Visual Studio 2013:
   1)	Open the game.dsp (VC++ 6 Project) and let it convert
   2)	Change the release type to "Release"
   3)	Compile
   4)	dll will be at "..\..\baseq2\gamex86.dll" (it will automatically overwrite the existing one)
   5)	Run

* Unlisted Versions of Visual Studio/Other Compilers: Untested
   It should be compatable, but they are not tested and are not supported

Playing the mod:
* Add/Change the following lines to config.cfg:
	bind 0 "use Mega Missile"
	bind 1 "use HyperBlaster"
	bind 2 "use Chaingun"
	bind 3 "use Blaster"
	bind 4 "use Machinegun"
	bind 5 "use Helix Cannon"
	bind 6 "use Rocket Launcher"
	bind 7 "use Homing Missile"
	bind 8 "use Grenade Launcher"
	bind 9 "use Smart Missile"
	bind SPACE "+strafeup"
	bind CTRL "+strafedown"

* Add the following lines to autoexec.cfg:
	alias +strafeup "strafey up"
	alias -strafeup "strafey off"
	alias +strafedown "strafey down"
	alias -strafedown "strafey off"

* Weapons:
   1)	Laser/Quad laser: Default weapon
		Use "give quadlaser", select and use from in game inventory to upgrade to quad laser
   2)	Vulcan Cannon:	Similar to the existing chaingun
		Find as pickup or use "give Chaingun"
   3)	Spreadfire
		Use "give Blaster" as pickups are not in existing maps
   4)	Plasma Cannon
		Find as pickup or use "give Machinegun"
   5)	Helix Cannon: enhanced version of spreadfire (bonus weapon from Descent 2)
		Use "give Helix Cannon" and select
   6)	Concussion Missile
		Find as pickup or use "give Rocket Launcher"
   7)	Homing Missile: Homing version of concussion missile
		Use "give Homing Missile" and select
   8)	Mines
		Find as pickup or use "give Grenade Launcher"
   9)	Smart Missile: Weapon is incomplete/does not function
		Use "give Smart Missile" and select
   0)	Mega Missile
		Use "give Mega Missile" and select

* Accessories:
   1)	Quadlaser upgrade: makes laser shoot 4 rounds instead of 2 per shot
		Use "give quadlaser", select and use from in game inventory to upgrade to quad laser
   2)	Ammo rack: doubles capacity of Vulcan Cannon/All Missiles/Mines
		Find as pickup or use "give bandolier", select and use from in game inventory