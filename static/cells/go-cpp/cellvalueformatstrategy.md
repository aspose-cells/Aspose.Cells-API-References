##CellValueFormatStrategy Enum
'CellValueFormatStrategy enum. Encapsulates the object that represents cellvalueformatstrategy in Go.'
## CellValueFormatStrategy Enum
Specifies how to apply style for the value of the cell.
```go
type CellValueFormatStrategy int32
```
## Fields
| Field | Description |
| --- | --- |
|[None](./none/) | Not formatted. |
|[CellStyle](./cellstyle/) | Only formatted with the cell's original style. |
|[DisplayStyle](./displaystyle/) | Formatted with the cell's displayed style. |
|[DisplayString](./displaystring/) | Gets the displayed string shown in ms excel.The main difference from <see cref="DisplayStyle"/> is this option also considers the effect of column width.If the column width is too small to show the formatted string completely,"#" may be shown, just like what ms excel does. |
