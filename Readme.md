### A collection of bugfixes

I would organize it in this way:
1) One mod for fixes in XML files.
2) One package of fixes for grahics.
Dividing it like this because graphic fixes might get very big in filesize (of course this mod also includes necessary xml changes to fix the graphics). So the graphic package will publish an update after modders added new fixes to it more seldom, to keep the downloadtraffic low. While the xml bugfix mod can be updated more often.

I think it is fine to include translation fixes within the XML bugfix mod, or do you think we should separate it?


### How to contribute:
- Either add your code/files directly into the mod.
- Or add your code/files as a submod: Simply create a normal mod, but name the folder a bit different, so users will notice that it is not a normal mod they need to handle, like eg "submod_bugfix_ABC_Serp". A submod is the better choice if you dont want to mix your work with others and if you also published a standalone version of your bugfix (then use the same ModID for both) so the game only loads one of it, if a user has both installed.

Please make sure to write your code as compatible as possible, eg. when you add a guid to a pool use a Condition to check if it is not already there:
```xml
<ModOp Type="add" GUID='1404' Path="/Values/ItemEffectTargetPool/EffectTargetGUIDs"
  Condition="!/Values/ItemEffectTargetPool/EffectTargetGUIDs/Item[GUID='720']">
  <Item>
    <GUID>720</GUID>
  </Item>
</ModOp>
```






Always up for suggestions, write us in the Anno modding discord:
https://discord.gg/nEQj3qfTYm
