```mermaid
classDiagram
direction LR
Game_BattlerBase"1"<|--"1"Game_Battler
Game_Battler"1"<|--"1"Game_Actor
Game_Actor"1"*--"0..n"Game_Item
Game_Battler"1"<|--"1"Game_Enemy
Game_Battler"1"*--"0..n"Game_Action
Game_Action"1"--"1"Game_Item
Game_Battler"1"--"1"Game_ActionResult
```
