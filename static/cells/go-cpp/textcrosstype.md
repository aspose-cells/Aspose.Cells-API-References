##TextCrossType Enum
'TextCrossType enum. Encapsulates the object that represents textcrosstype in Go.'
## TextCrossType Enum
Enumerates displaying text type when the text width is larger than cell width.
```go
type TextCrossType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Default](./default/) | Display text like in Microsoft Excel. |
|[CrossKeep](./crosskeep/) | Display all the text by crossing other cells and keep text of crossed cells. |
|[CrossOverride](./crossoverride/) | Display all the text by crossing other cells and override text of crossed cells. |
|[StrictInCell](./strictincell/) | Only display the text within the width of cell. |
