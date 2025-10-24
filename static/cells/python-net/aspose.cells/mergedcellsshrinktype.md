##MergedCellsShrinkType enumeration
## MergedCellsShrinkType enumeration
Represents the strategy to shrink merged cells for operations such as deleting blank rows/column.
The MergedCellsShrinkType type exposes the following members:
### Fields
| Field | Description |
| :- | :- |
| NONE | Leaves the merged cells as it is without any modification. |
| SHRINK_TO_FIT | Shrinks the merged area if needed, by removing rows from the bottom or columns from the right,
| KEEP_HEADER_ONLY | Only keeps the header rows/columns of the merged area when the top-left cell of the merged area is not blank. |
### See Also
* module [`aspose.cells`](..)
