##PlacementType Enum
'PlacementType enum. Encapsulates the object that represents placementtype in Go.'
## PlacementType Enum
Represents the way the drawing object is attached to the cells below it.
```go
type PlacementType int32
```
## Fields
| Field | Description |
| --- | --- |
|[FreeFloating](./freefloating/) | Don't move or size with cells. |
|[Move](./move/) | Move but don't size with cells. |
|[MoveAndSize](./moveandsize/) | Move and size with cells. |
