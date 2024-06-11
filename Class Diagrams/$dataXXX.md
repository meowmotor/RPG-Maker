|Variable Name|Filename|Path on your editor|
|---|---|---|
|$dataActors|Actors.json|Database > Actors|
|$dataClasses|Classes.json|Database > Classes|
|$dataSkills|Skills.json|Database > Skills|
|$dataItems|Items.json|Database > Items|
|$dataWeapons|Weapons.json|Database > Weapons|
|$dataArmors|Armors.json|Database > Armors|
|$dataEnemies|Enemies.json|Database > Enemies|
|$dataTroops|Troops.json|Database > Troops|
|$dataStates|States.json|Database > States|
|$dataAnimations|Animations.json|Database > Animations|
|$dataTilesets|Tilesets.json|Database > Tilesets|
|$dataCommonEvents|CommonEvents.json|Database > Common Events|
|$dataSystem|System.json|Database > System 1/2|
|$dataMapInfos|MapInfos.json|Database > MapInfos|

```mermaid
classDiagram
direction LR
`$dataActors`<--Game_Actor:actor()
`$dataClasses`<--Game_Actor:currentClass()
`$dataSkills`<--Game_Item:object()
`$dataItems`<--Game_Item:object()
`$dataWeapons`<--Game_Item:object()
`$dataArmors`<--Game_Item:object()
`$dataItems`<--Game_Enemy:itemObject()
`$dataWeapons`<--Game_Enemy:itemObject()
`$dataArmors`<--Game_Enemy:itemObject()
`$dataItems`<--Window_ShopBuy:goodsToItem()
`$dataWeapons`<--Window_ShopBuy:goodsToItem()
`$dataArmors`<--Window_ShopBuy:goodsToItem()
`$dataEnemies`<--Game_Enemy:enemy()
`$dataTroops`<--Game_Troop:troop()
`$dataStates`<--Game_BattlerBase:states()
`$dataAnimation`<--Sprite_Animation:_animation
`$dataAnimation`<--Sprite_AnimationMV:_animation
`$dataTilesets`<--Game_Map:tileset()
`$dataCommonEvents`<--Game_Temp:retrieveCommonEvent()
`$dataCommonEvents`<--Game_CommonEvent:event()
`$dataSystem`
`$dataMapInfos`
`$dataMap`
```
