##Worksheet.Unmerge
Worksheet method. Unmerges a specified range of cells into a single cell
## Unmerge(CellRange) {#unmerge_1}
Unmerges a specified range of cells into a single cell.
```csharp
public void Unmerge(CellRange r)
```
| Parameter | Type | Description |
| --- | --- | --- |
| r | CellRange | CellRange of this range(zero based) |
### Remarks
Reference the merged cell via the address of the upper-left cell in the range.
### See Also
* class [CellRange](../../cellrange/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Unmerge(CellLocation) {#unmerge}
Remove the specified cell location from merges.
```csharp
public void Unmerge(CellLocation location)
```
| Parameter | Type | Description |
| --- | --- | --- |
| location | CellLocation | Cell location. |
### See Also
* class [CellLocation](../../celllocation/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Unmerge(int, int) {#unmerge_2}
Remove the specified cell row column index from merges.
```csharp
public void Unmerge(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| column | Int32 | Column index. |
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
