##Aspose::Cells::Cell::GetStringValue method
'Aspose::Cells::Cell::GetStringValue method. Gets the string value by specific formatted strategy in C++.'
## Cell::GetStringValue(CellValueFormatStrategy) method
Gets the string value by specific formatted strategy.
```cpp
U16String Aspose::Cells::Cell::GetStringValue(CellValueFormatStrategy formatStrategy)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formatStrategy | CellValueFormatStrategy | The formatted strategy. |
## ReturnValue
## See Also
* Class [U16String](../../u16string/)
* Enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::GetStringValue() method
Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself. For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned. The formatted cell value is same with what you can get from excel when copying a cell as text(such as copying cell to text editor or exporting to csv).
```cpp
U16String Aspose::Cells::Cell::GetStringValue()
```
## See Also
* Class [U16String](../../u16string/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
