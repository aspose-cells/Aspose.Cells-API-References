##WebCells.SetStyle
WebCells method. Sets the style to a specified range of cells
## SetStyle(int, int, int, int, TableItemStyle) {#setstyle}
Sets the style to a specified range of cells.
```csharp
public void SetStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber,
TableItemStyle style)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of this range(zero based) |
| firstColumn | Int32 | First column of this range(zero based) |
| rowNumber | Int32 | Number of rows(one based) |
| columnNumber | Int32 | Number of columns(one based) |
| style | TableItemStyle | The style object to be set |
### See Also
* class [TableItemStyle](../../../aspose.cells.gridweb/tableitemstyle/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
## SetStyle(string, TableItemStyle) {#setstyle_1}
Sets the style to a specified range of cells.
```csharp
public void SetStyle(string cellRange, TableItemStyle style)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellRange | String | The range of cells' names, like "A1:D6" |
| style | TableItemStyle | The style object to be set |
### See Also
* class [TableItemStyle](../../../aspose.cells.gridweb/tableitemstyle/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
