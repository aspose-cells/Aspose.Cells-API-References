##Aspose::Cells::Cells::Merge method
'Aspose::Cells::Cells::Merge method. Merges a specified range of cells into a single cell in C++.'
## Cells::Merge(int32_t, int32_t, int32_t, int32_t) method
Merges a specified range of cells into a single cell.
```cpp
void Aspose::Cells::Cells::Merge(int32_t firstRow, int32_t firstColumn, int32_t totalRows, int32_t totalColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int32_t | First row of this range(zero based) |
| firstColumn | int32_t | First column of this range(zero based) |
| totalRows | int32_t | Number of rows(one based) |
| totalColumns | int32_t | Number of columns(one based) |
## Remarks
Reference the merged cell via the address of the upper-left cell in the range.
## See Also
* Class [Vector](../../vector/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cells::Merge(int32_t, int32_t, int32_t, int32_t, bool) method
Merges a specified range of cells into a single cell.
```cpp
void Aspose::Cells::Cells::Merge(int32_t firstRow, int32_t firstColumn, int32_t totalRows, int32_t totalColumns, bool mergeConflict)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int32_t | First row of this range(zero based) |
| firstColumn | int32_t | First column of this range(zero based) |
| totalRows | int32_t | Number of rows(one based) |
| totalColumns | int32_t | Number of columns(one based) |
| mergeConflict | bool | Merge conflict merged ranges. |
## Remarks
Reference the merged cell via the address of the upper-left cell in the range. If mergeConflict is true and the merged range conflicts with other merged cells, other merged cells will be automatically removed.
## See Also
* Class [Vector](../../vector/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cells::Merge(int32_t, int32_t, int32_t, int32_t, bool, bool) method
Merges a specified range of cells into a single cell.
```cpp
void Aspose::Cells::Cells::Merge(int32_t firstRow, int32_t firstColumn, int32_t totalRows, int32_t totalColumns, bool checkConflict, bool mergeConflict)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int32_t | First row of this range(zero based) |
| firstColumn | int32_t | First column of this range(zero based) |
| totalRows | int32_t | Number of rows(one based) |
| totalColumns | int32_t | Number of columns(one based) |
| checkConflict | bool | Indicates whether check the merged cells intersects other merged cells |
| mergeConflict | bool | Merge conflict merged ranges. |
## Remarks
Reference the merged cell via the address of the upper-left cell in the range. If mergeConflict is true and the merged range conflicts with other merged cells, other merged cells will be automatically removed.
## See Also
* Class [Vector](../../vector/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
