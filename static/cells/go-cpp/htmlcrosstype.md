##HtmlCrossType Enum
'HtmlCrossType enum. Encapsulates the object that represents htmlcrosstype in Go.'
## HtmlCrossType Enum
Represents five types of html cross string.
```go
type HtmlCrossType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Default](./default/) | Display like MS Excel,depends on the next cell.If the next cell is null,the string will cross,or it will be truncated |
|[MSExport](./msexport/) | Display the string like MS Excel exporting html. |
|[Cross](./cross/) | Display HTML cross string, this performance for creating large html files will be more than ten times faster than setting the value to Default or FitToCell. |
|[CrossHideRight](./crosshideright/) | Display HTML cross string and hide the right string when the texts overlap. |
|[FitToCell](./fittocell/) | Only displaying the string within the width of cell. |
