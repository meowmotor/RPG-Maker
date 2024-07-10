```mermaid
classDiagram
direction LR
`PIXI.Point`<|--Point
`PIXI.Rectangle`<|--Rectangle
`PIXI.Sprite`<|--Sprite
`PIXI.Container`<|--Tilemap
Tilemap<|--ShaderTilemap
`PIXI.extras.PictureTilingSprite`<|--TilingSprite
`PIXI.Container`<|--ScreenSprite
`PIXI.Container`<|--Window
`PIXI.Container`<|--WindowLayer
`PIXI.Container`<|--Weather
`PIXI.filters.ColorMatrixFilter`<|--ToneFilter
`PIXI.Container`<|--ToneSprite
`PIXI.Container`<|--Stage
```
