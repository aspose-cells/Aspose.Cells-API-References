##PaneStateType Enum
'PaneStateType enum. Encapsulates the object that represents panestatetype in Go.'
## PaneStateType Enum
Represents state of the sheet's pane.
```go
type PaneStateType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Frozen](./frozen/) | Panes are frozen, but were not before being frozen. |
|[FrozenSplit](./frozensplit/) | Panes are frozen and were split before being frozen. |
|[Split](./split/) | Panes are split, but not frozen. |
|[Normal](./normal/) | Panes are not frozen and not split. |
