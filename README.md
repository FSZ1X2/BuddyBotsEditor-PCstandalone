Info:  
The location of the bot.pk4’s are in the d3xp\botPaks  
Each of the pk4’s contain a bot.def and a bot.py  
The name of the bot must be uniform across all files (which includes capitalizations).  

How to create your bots:  
Step-1:  
enter your name and your bot name on the left  
Step-2:  
click the "QuickStart" button on the bottom to get the basic struct of bots code  
Step-3:  
drag and drop the functions or commands to complete your bot  
Step-4:  
click the "Export" button to export and save your bot to your disk  

Functions and command:  
bool InView(IdEntity* entity)  
 -Returns wether the entity passed in is in view or not  
List<Entity*> FindNearbyPlayers()  
 -Returns a list of idPlayer that are in the bots line of sight  
List<Entity*> FindItemsInView()  
 -Returns a list of idEntity that are in the bots line of sight  
MoveToPosition(vec3 pos, int range)  
 -Tells bot to move to this position and the range is for ???  
LookAtPosition(vec3 pos)  
 -Tells bot to look at this position  
Attack()  
 -Tells bot to start firing weapon (will switch to other weapons if out of ammo, except for fists)  
StopAttack()  
 -Tells bot to stop firing weapon  
Entity* FindItem(const char* item)  
 -Goes through entity list to find all items of that name on that map. Returns the first one found in the list.  
int HasAmmo(const char* weaponName)  
 -Returns how much ammo the weapon passed in has.  
bool SwitchWeapon(const char* weaponName)  
 -Returns weather or not the passed in weapon name is available to equip, if it is, it will be equip.  
AmmoInClip()  
 -Checks if the current equipped weapon has ammo in the current clip. If it doesn't, it will reload the weapon.  
UpdateAiMoveFlag(aiMoveFlag_t flag)  
 -Changes the movement state of the AI  

AiMove Flags:  
NULLMOVE  
 -Stops moving  
CROUCH  
JUMP  
 -Doesn't work as of this moment  
WALK  
RUN  

Weapon List:  
weapon_flashlight  
weapon_pistol  
weapon_machinegun_mp  
weapon_shotgun  
weapon_rocketlauncher  
weapon_handgrenade  
weapon_chainsaw  
weapon_fists       

Item List:  
item_medkit  
item_medkit_small  

Console Commands:  
Addbot  
 -Adds the bot typed to the play queue  
 -Ex. Addbot samplebot  
Removebot  
 -Remove the bot typed from the queue  
 -Ex. Removebot samplebot  
Removeallbots  
 -Remove all bots from the queue  
Addteam  
 -Add the team typed to the play queue. They will be forced into a team when the game.  
 -Ex. Addteam lightside  
Removeallteams  
 -Removes all teams from the play queue. If there is a team in the queue, it must be removed by this command.  
Removebotindex  
 -Remove specific bot from the queue. The index is giving with the printallbots as well as what list it is on.  
 -Ex. Removebotindex list2 1  
Printallbots  
 -Prints all the bots currently in the play queue  


update 03/17/2017
added the basic setup of standalone version

update 03/20/2017
the way to run buddybots editor:
download and install electron on your computer
(Also, you can download the prebuild version of electron then drag the app folder to run the application)
open the command window and do "npm install jszip"
