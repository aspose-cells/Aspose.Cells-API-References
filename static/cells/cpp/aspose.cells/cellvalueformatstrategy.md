##Aspose::Cells::CellValueFormatStrategy enum
'Aspose::Cells::CellValueFormatStrategy enum. Specifies how to apply style for the value of the cell in C++.'
## CellValueFormatStrategy enum
Specifies how to apply style for the value of the cell.
```cpp
enum class CellValueFormatStrategy
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | 0 | <br>Not formatted. |
| CellStyle | 1 | <br>Only formatted with the cell's original style. |
| DisplayStyle | 2 | <br>Formatted with the cell's displayed style. |
| DisplayString | 3 | <br>Gets the displayed string shown in ms excel. The main difference from [DisplayStyle](./) is this option also considers the effect of column width. If the column width is too small to show the formatted string completely, "#" may be shown, just like what ms excel does. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
