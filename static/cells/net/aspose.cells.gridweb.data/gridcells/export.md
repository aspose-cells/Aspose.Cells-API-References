##GridCells.Export
GridCells method. Exports data in the Cells collection of a WebWorksheet to a new DataTable object
## GridCells.Export method
Exports data in the Cells collection of a WebWorksheet to a new DataTable object
```csharp
public DataTable Export(int startRow, int startColumn, int rows, int columns,
bool exportColumnName, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The row number of the first cell to export out. |
| startColumn | Int32 | The column number of the first cell to export out. |
| rows | Int32 | Number of rows to be imported. |
| columns | Int32 | Number of columns to be imported. |
| exportColumnName | Boolean | Indicates whether the data in the first row are exported as the column name of the DataTable |
| isVertical | Boolean | True if a row in Excel file represents a row in DataTable. False if a column in Excel file represents a row in DataTable. |
### Return Value
Exported DataTable object.
### See Also
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
