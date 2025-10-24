##GridCells.SetStyle
GridCells method. Sets the style to a specified range of cells
## SetStyle(int, int, int, int, Style) {#setstyle_1}
Sets the style to a specified range of cells.
```csharp
public void SetStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, Style style)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of this range(zero based) |
| firstColumn | Int32 | First column of this range(zero based) |
| rowNumber | Int32 | Number of rows(one based) |
| columnNumber | Int32 | Number of columns(one based) |
| style | Style | The style object to be set |
### See Also
* class [Style](../../../aspose.cells.griddesktop/style/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## SetStyle(string, Style) {#setstyle_2}
Sets the style to a specified range of cells.
```csharp
public void SetStyle(string cellRange, Style style)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellRange | String | The range of cells' names, like "A1:D6" |
| style | Style | The style object to be set |
### See Also
* class [Style](../../../aspose.cells.griddesktop/style/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## SetStyle(CellRange, Style) {#setstyle}
Sets the style to a specified range of cells.
```csharp
public void SetStyle(CellRange cellRange, Style style)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellRange | CellRange | The range of cells |
| style | Style | The style object to be set |
### See Also
* class [CellRange](../../../aspose.cells.griddesktop/cellrange/)
* class [Style](../../../aspose.cells.griddesktop/style/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
