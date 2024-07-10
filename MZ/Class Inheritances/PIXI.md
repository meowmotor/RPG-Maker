```mermaid
classDiagram
direction LR
`PIXI.Point`<|--Point
`PIXI.Rectangle`<|--Rectangle
`PIXI.Sprite`<|--Sprite
`PIXI.Container`<|--ScreenSprite
`PIXI.Container`<|--Window
`PIXI.Container`<|--WindowLayer
`PIXI.Container`<|--Weather
`PIXI.Container`<|--Stage
`PIXI.Container`<|--Tilemap
`PIXI.Container`<|--`Tilemap.Layer`
`PIXI.Container`<|--`Tilemap.CombinedLayer`
`PIXI.ObjectRenderer`<|--`Tilemap.Renderer`
`PIXI.TilingSprite`<|--TilingSprite
`PIXI.Filter`<|--ColorFilter
```
