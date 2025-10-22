##GridCells.Item
GridCells property. Gets the GridCell element at the specified cell row index and column index
## GridCells indexer (1 of 2)
Gets the [`GridCell`](../../gridcell/) element at the specified cell row index and column index.
```csharp
public GridCell this[int row, int column] { get; }
```
| Parameter | Description |
| --- | --- |
| row | Row index. |
| column | Column index. |
### Return Value
The [`GridCell`](../../gridcell/) object.
### Examples
```csharp
[C#]
Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells[0, 0];	//Gets the cell at "A1"
[Visual Basic]
Dim cells As Cells =  excel.WorkSheets(0).Cells
Dim cell As Cell =  cells(0,0)  'Gets the cell at "A1"
```
### See Also
* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## GridCells indexer (2 of 2)
Gets the [`GridCell`](../../gridcell/) element at the specified cell name.
```csharp
public GridCell this[string cellName] { get; }
```
| Parameter | Description |
| --- | --- |
| cellName | Cell name,including its column letter and row number, for example A5. |
### Return Value
A [`GridCell`](../../gridcell/) object
### See Also
* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
