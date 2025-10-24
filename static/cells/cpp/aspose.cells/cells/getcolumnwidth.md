##Aspose::Cells::Cells::GetColumnWidth method
'Aspose::Cells::Cells::GetColumnWidth method. Gets the column width in C++.'
## Cells::GetColumnWidth(int32_t, bool, CellsUnitType) method
Gets the column width.
```cpp
double Aspose::Cells::Cells::GetColumnWidth(int32_t column, bool isOriginal, CellsUnitType unitType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | int32_t | The column index. |
| isOriginal | bool | Indicates whether getting original width. |
| unitType | CellsUnitType |  |
## ReturnValue
## See Also
* Class [Vector](../../vector/)
* Enum [CellsUnitType](../../cellsunittype/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cells::GetColumnWidth(int32_t) method
Gets the width(in unit of characters) of the specified column in normal view.
```cpp
double Aspose::Cells::Cells::GetColumnWidth(int32_t column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | int32_t | [Column](../../column/) index |
## ReturnValue
Width of column. For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.
## See Also
* Class [Vector](../../vector/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
