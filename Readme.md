### A collection of bugfixes

THIS is still WIP! Renaming and Restructure will for sure happen and is open for discussion at discord!
But you can already contribute.

If you are not sure if your mod is a "Fix" or "personal taste" or if it is the best way to fix it, we can discuss at discord if we should include it or not. You may put your code into the "ChangesOpenForDiscussion" folder.

If your fix has negative consequences that not every user would like to accept (eg. it is more a workaround, not a real fix), you should make it a separate mod, so users can decide if they want it or not.

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
