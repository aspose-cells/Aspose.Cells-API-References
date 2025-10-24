##Aspose::Cells::Cells::GetCellDisplayStyle method
'Aspose::Cells::Cells::GetCellDisplayStyle method. Get the display style of given cell in C++.'
## Cells::GetCellDisplayStyle(int32_t, int32_t) method
Get the display style of given cell.
```cpp
Style Aspose::Cells::Cells::GetCellDisplayStyle(int32_t row, int32_t column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | int32_t | row index of given cell |
| column | int32_t | column of given cell |
## ReturnValue
the display style of given cell.
## Remarks
Same with [Cell.GetDisplayStyle()](../../cell/getdisplaystyle/), and same with using [BorderType.SideBorders](../../bordertype/) for [GetCellDisplayStyle(int, int, BorderType)](./).
## See Also
* Class [Style](../../style/)
* Class [Vector](../../vector/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cells::GetCellDisplayStyle(int32_t, int32_t, BorderType) method
Get the display style of given cell.
```cpp
Style Aspose::Cells::Cells::GetCellDisplayStyle(int32_t row, int32_t column, BorderType adjacentBorders)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | int32_t | row index of given cell |
| column | int32_t | column of given cell |
| adjacentBorders | BorderType | Indicates which borders need to be checked and adjusted according to the borders of adjacent cells. Please see the description for the same parameter of [Cell.GetDisplayStyle(BorderType)](../../cell/getdisplaystyle/). |
## ReturnValue
the display style of given cell.
## Remarks
If the cell is also affected by other settings such as conditional formatting, list objects, etc., then the display style may be different from [GetCellStyle(int, int)](../getcellstyle/). And because those settings also may be applied to empty(non-existing) cells, using this method can avoid the instantiation of those empty cells so the performance will be better than getting the [Cell](../../cell/) instance from [Cells](../) and then calling [Cell.GetDisplayStyle(BorderType)](../../cell/getdisplaystyle/).
## See Also
* Class [Style](../../style/)
* Class [Vector](../../vector/)
* Enum [BorderType](../../bordertype/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
