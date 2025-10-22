##MergedCellsShrinkType Enum
'MergedCellsShrinkType enum. Encapsulates the object that represents mergedcellsshrinktype in Go.'
## MergedCellsShrinkType Enum
Represents the strategy to shrink merged cells for operations such as deleting blank rows/column.
```go
type MergedCellsShrinkType int32
```
## Fields
| Field | Description |
| --- | --- |
|[None](./none/) | Leaves the merged cells as it is without any modification. |
|[ShrinkToFit](./shrinktofit/) | Shrinks the merged area if needed, by removing rows from the bottom or columns from the right,while ensuring all content remains visible. |
|[KeepHeaderOnly](./keepheaderonly/) | Only keeps the header rows/columns of the merged area when the top-left cell of the merged area is not blank. |
