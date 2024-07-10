|Variable Name|Type|
|---|---|
|$gameTemp|Game_Temp|
|$gameSystem|Game_System|
|$gameScreen|Game_Screen|
|$gameTimer|Game_Timer|
|$gameMessage|Game_Message|
|$gameSwitches|Game_Switches|
|$gameVariables|Game_Variables|
|$gameSelfSwitches|Game_SelfSwitches|
|$gameActors|Game_Actors|
|$gameParty|Game_Party|
|$gameTroop|Game_Troop|
|$gameMap|Game_Map|
|$gamePlayer|Game_Player|

```mermaid
classDiagram
direction LR
class `$gameTemp`
class `$gameSystem`
class `$gameScreen`
class `$gameTimer`
class `$gameMessage`
class `$gameSwitches`
class `$gameVariables`
class `$gameSelfSwitches`
class `$gameActors`
`$gameParty`<--Game_Actor:friendsUnit()
`$gameParty`<--Game_Enemy:opponentsUnit()
`$gameTroop`<--Game_Actor:opponentsUnit()
`$gameTroop`<--Game_Enemy:friendsUnit()
class `$gameMap`
`$gamePlayer`<--Game_Interpreter:character()
```
