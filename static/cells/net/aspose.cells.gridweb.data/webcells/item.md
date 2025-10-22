##WebCells.Item
WebCells property. Gets the Cell element at the specified cell row index and column index
## WebCells indexer (1 of 2)
Gets the Cell element at the specified cell row index and column index.
```csharp
public WebCell this[int row, int column] { get; }
```
| Parameter | Description |
| --- | --- |
| row | Row index. |
| column | Column index. |
### Return Value
The Cell object.
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
* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
## WebCells indexer (2 of 2)
Gets the Cell element at the specified cell name.
```csharp
public WebCell this[string cellName] { get; }
```
| Parameter | Description |
| --- | --- |
| cellName | Cell name,including its column letter and row number, for example A5. |
### Return Value
A Cell object
### Examples
```csharp
[C#]
Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells["A1"];	//Gets the cell at "A1"
[Visual Basic]
Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```
### See Also
* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
