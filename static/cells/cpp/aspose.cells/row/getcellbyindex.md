##Aspose::Cells::Row::GetCellByIndex method
'Aspose::Cells::Row::GetCellByIndex method. Get the cell by specific index in the cells collection of this row in C++.'
## Row::GetCellByIndex method
Get the cell by specific index in the cells collection of this row.
```cpp
Cell Aspose::Cells::Row::GetCellByIndex(int32_t index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t | The index(position) of the cell in the cells collection of this row. |
## ReturnValue
The [Cell](../../cell/) object at given position.
## Remarks
To traverse all cells in sequence without modification, using [GetEnumerator()](../getenumerator/) will give better performance than using this method to get cell one by one.
## See Also
* Class [Cell](../../cell/)
* Class [Vector](../../vector/)
* Class [Row](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
