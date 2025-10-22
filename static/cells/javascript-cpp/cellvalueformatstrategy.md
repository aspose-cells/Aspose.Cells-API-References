##CellValueFormatStrategy
Specifies how to apply style for the value of the cell.
## CellValueFormatStrategy enumeration
Specifies how to apply style for the value of the cell.
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Not formatted. |
| CellStyle | `1` | Only formatted with the cell's original style. |
| DisplayStyle | `2` | Formatted with the cell's displayed style. |
| DisplayString | `3` | Gets the displayed string shown in ms excel. The main difference from [DisplayStyle](../displaystyle/) is this option also considers the effect of column width. If the column width is too small to show the formatted string completely, "#" may be shown, just like what ms excel does. |
