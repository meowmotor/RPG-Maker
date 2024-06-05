```mermaid
classDiagram
direction LR
Game_Unit"1"<|--"1"Game_Party
Game_Unit"1"<|--"1"Game_Troop
Game_Party"1"*--"1"Game_Item:_lastItem
Game_Party"1"-->"0..*"Game_Actor:_actors
Game_Actors"1"-->"0..*"Game_Actor:_data
Game_BattlerBase"1"<|--"1"Game_Battler
Game_Battler"1"<|--"1"Game_Actor
Game_Actor"1"-->"0..*"Game_Item:_skills
Game_Actor"1"*--"0..*"Game_Item:_equips
Game_Actor"1"*--"1"Game_Item:_lastMenuSkill, _lastBattleSkill
Game_Battler"1"<|--"1"Game_Enemy
Game_Battler"1"*--"0..*"Game_Action:_actions
Game_Action"1"*--"1"Game_Item:_item
Game_Action"1"-->"1"Game_Actor:subject()
Game_Action"1"-->"1"Game_Enemy:subject()
Game_Battler"1"*--"1"Game_ActionResult:_result
Game_Troop"1"-->"0..*"Game_Enemy:_enemies
Game_Troop"1"*--"1"Game_Interpreter:_interpreter
```
