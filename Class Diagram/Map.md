```mermaid
classDiagram
direction LR
Game_Map"1"*--"1"Game_Interpreter:_interpreter
Game_Map"1"*--"0..*"Game_Vehicle:_vehicles
Game_Map"1"*--"0..*"Game_Event:_events
Game_Map"1"*--"0..*"Game_CommonEvent:_commonEvents
Game_CommonEvent"1"*--"1"Game_Interpreter:_interpreter
```
