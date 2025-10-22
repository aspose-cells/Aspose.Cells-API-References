##Cells.ImportDataGridAsString
Cells method. Imports a DataGrid into a worksheet. This method doesnt try to convert text into numeric values
## Cells.ImportDataGridAsString method
Imports a DataGrid into a worksheet. This method doesn't try to convert text into numeric values.
```csharp
public int ImportDataGridAsString(DataGrid dataGrid, int firstRow, int firstColumn, bool insertRows)
```
| Parameter | Type | Description |
| --- | --- | --- |
| dataGrid | DataGrid | The DataGrid object to be imported. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| insertRows | Boolean | Indicates whether extra rows are added to fit data. |
### Return Value
Total number of rows imported
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
