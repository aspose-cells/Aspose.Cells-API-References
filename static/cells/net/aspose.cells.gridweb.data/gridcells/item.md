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
GridWeb GridWeb1 = new GridWeb();
GridCells cells = GridWeb1.WorkSheets[0].Cells;
//Gets the cell at "A1"
GridCell cell = cells[0, 0];
[Visual Basic]
Dim cells As Cells =  excel.WorkSheets(0).Cells
'Gets the cell at "A1"
Dim cell As Cell =  cells(0,0)
```
### See Also
* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
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
### Examples
```csharp
[C#]
ridWeb GridWeb1 = new GridWeb();
GridCells cells = GridWeb1.WorkSheets[0].Cells;
GridCell cell = cells["A1"];	//Gets the cell at "A1"
[Visual Basic]
Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```
### See Also
* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
