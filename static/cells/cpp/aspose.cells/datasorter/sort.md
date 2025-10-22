##Aspose::Cells::DataSorter::Sort method
'Aspose::Cells::DataSorter::Sort method. Sorts the data of the area in C++.'
## DataSorter::Sort(const Cells\&, int32_t, int32_t, int32_t, int32_t) method
Sorts the data of the area.
```cpp
Vector<int32_t> Aspose::Cells::DataSorter::Sort(const Cells &cells, int32_t startRow, int32_t startColumn, int32_t endRow, int32_t endColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cells | const Cells\& | The cells contains the data area. |
| startRow | int32_t | The start row of the area. |
| startColumn | int32_t | The start column of the area. |
| endRow | int32_t | The end row of the area. |
| endColumn | int32_t | The end column of the area. |
## ReturnValue
the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.
## See Also
* Class [Vector](../../vector/)
* Class [Cells](../../cells/)
* Class [DataSorter](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## DataSorter::Sort(const Cells\&, const CellArea\&) method
Sort the data of the area.
```cpp
Vector<int32_t> Aspose::Cells::DataSorter::Sort(const Cells &cells, const CellArea &area)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cells | const Cells\& | The cells contains the data area. |
| area | const CellArea\& | The area needed to sort |
## ReturnValue
the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.
## See Also
* Class [Vector](../../vector/)
* Class [Cells](../../cells/)
* Class [CellArea](../../cellarea/)
* Class [DataSorter](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## DataSorter::Sort() method
Sort the data in the range.
```cpp
Vector<int32_t> Aspose::Cells::DataSorter::Sort()
```
## ReturnValue
the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.
## See Also
* Class [Vector](../../vector/)
* Class [DataSorter](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
