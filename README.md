# Incubus at home:
"Incubus At Home" is a stupid, stinky, and janky library I coded and farted out of my butt in just a few days. It was made out of pure boredom.
This library is an installable version of the Dynamic Minisaacs Forever! mod, inspired by KittenChilly's Dynamic Minisaac Tears mod, and programmed by me.

## HOW THE FUCK DO I USE THIS THING???

Do this in the main.lua:
```lua
GLOBAL_VARIABLE = RegisterMod("The Coolest Motherfucking Mod Ever", 1)
GLOBAL_VARIABLE.SaveManager = include("path.to.savemanager")
--May look different depending on how you installed the save manager.
GLOBAL_VARIABLE.MimicShitNow = include("path.to.incubus_at_home")
```
Then return to the library's lua file and do the following to these variables:

```lua
local ModReference = "Insert your mod's global variable here"
local savemanager = "Insert your mod's save manager variable here"
```

>"GLOBAL_VARIABLE" should replace "Insert your mod's global variable here"
>Replace "Insert your mod's save manager variable here" with "GLOBAL_VARIABLE.SaveManager".

>Do NOT copy the quotation marks!
(This lib only works with Catinsurance's SaveManager because I fucking suck at programming. I'm sorry.)

If you want to spawn a mimicking minisaac, do the following:

```lua
GLOBAL_VARIABLE.MimicShitNow:AddIncubusAtHome(EntityPlayer, MinisaacPosition)
```
Treat this like the base api's AddMinisaac(), without the playanim argument.
This function returns an EntityFamiliar Object.
If both arguments are nil, spawns a mimicking Minisaac that mimics P1 at P1's Position by default.
DO NOT MESS WITH THE MINISAACS' KEY COUNT(EntityFamiliar.Keys)!
