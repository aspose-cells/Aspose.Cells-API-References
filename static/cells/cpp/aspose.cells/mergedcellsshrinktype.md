##Aspose::Cells::MergedCellsShrinkType enum
'Aspose::Cells::MergedCellsShrinkType enum. Represents the strategy to shrink merged cells for operations such as deleting blank rows/column in C++.'
## MergedCellsShrinkType enum
Represents the strategy to shrink merged cells for operations such as deleting blank rows/column.
```cpp
enum class MergedCellsShrinkType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | 0 | <br>Leaves the merged cells as it is without any modification. |
| ShrinkToFit | 1 | <br>Shrinks the merged area if needed, by removing rows from the bottom or columns from the right, while ensuring all content remains visible. |
| KeepHeaderOnly | 2 | <br>Only keeps the header rows/columns of the merged area when the top-left cell of the merged area is not blank. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
