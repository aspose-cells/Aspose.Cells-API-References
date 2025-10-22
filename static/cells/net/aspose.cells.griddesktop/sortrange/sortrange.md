##SortRange.SortRange
SortRange constructor. Intializes a new instance of the SortRange class by specifing a worksheet range and sort orientation
## SortRange constructor
Intializes a new instance of the [`SortRange`](../) class by specifing a worksheet range and sort orientation.
```csharp
public SortRange(Worksheet worksheet, int startRow, int startColumn, int rows, int columns,
SortOrientation orientation, bool isCaseSensitive)
```
| Parameter | Type | Description |
| --- | --- | --- |
| worksheet | Worksheet | The Worksheet that contains the range. |
| startRow | Int32 | The start row of the range. |
| startColumn | Int32 | The start column of the range. |
| rows | Int32 | The number of the rows. |
| columns | Int32 | The number of the columns |
| orientation | SortOrientation | The sort orientation: top to bottom or left to right. |
| isCaseSensitive | Boolean | Determines whether the sort datas is case sensitive if datas are string |
### See Also
* class [Worksheet](../../worksheet/)
* enum [SortOrientation](../../sortorientation/)
* class [SortRange](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
