##Worksheet.ExportDataTable
Worksheet method. Exports data in the Cells collection of a Worksheet to a specifed DataTable object
## ExportDataTable(int, int, int, int, bool) {#exportdatatable_1}
Exports data in the Cells collection of a Worksheet to a specifed DataTable object.
```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns,
bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The row number of the first cell to export out. |
| startColumn | Int32 | The column number of the first cell to export out. |
| rows | Int32 | Number of rows to be imported. |
| columns | Int32 | Number of columns to be imported. |
| isVertical | Boolean | True if a row in the control represents a row in DataTable. False if a column in the control represents a row in DataTable. |
### Return Value
Exported DataTable object.
### Remarks
The method permits first create a DataTable object. Then exports data to the DataTable object. If dataTable don't be set valid, the method will return a new DataTable object by calling overload method 'Export(bool exportColumnName, bool isVertical)'.
### Examples
```csharp
[C#]
DataTable dataTable = new DataTable();
dataTable.Columns.Add("Column a",System.Type.GetType("System.String"));
dataTable.Columns.Add("Column b");
dataTable.Columns.Add("Column c");
dataTable.Columns.Add("Column d",System.Type.GetType("System.Double"));
dataTable.Columns.Add("Column e",System.Type.GetType("System.Int32"));
dataTable.Columns.Add("Column f",System.Type.GetType("System.Int32"));
DataTable exportTable = gridDesktop.Worksheets[0].Export(dataTable,1,0,10,6,true);
DataGrid1.SetDataBinding(exportTable, null);
[VB]
Dim dataTable As DataTable =  New DataTable()
dataTable.Columns.Add("Column a",System.Type.GetType("System.String"))
dataTable.Columns.Add("Column b")
dataTable.Columns.Add("Column c")
dataTable.Columns.Add("Column d",System.Type.GetType("System.Double"))
dataTable.Columns.Add("Column e",System.Type.GetType("System.Int32"))
dataTable.Columns.Add("Column f",System.Type.GetType("System.Int32"))
Dim exportTable As DataTable =  GridDesktop.Worksheets(0).Export(dataTable,1,0,10,6,True)
DataGrid1.SetDataBinding(exportTable)
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## ExportDataTable(int, int, int, int, bool, bool) {#exportdatatable_2}
Exports data in the Cells collection of a Worksheet to a new DataTable object.
```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns,
bool exportColumnName, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The row number of the first cell to export out. |
| startColumn | Int32 | The column number of the first cell to export out. |
| rows | Int32 | Number of rows to be imported. |
| columns | Int32 | Number of columns to be imported. |
| exportColumnName | Boolean | Indicates whether the data in the first row are exported to the column name of the DataTable. |
| isVertical | Boolean | True if a row in the control represents a row in DataTable. False if a column in the control represents a row in DataTable. |
### Return Value
Exported DataTable object.
### Examples
```csharp
[C#]
DataTable exportTable = gridDesktop.Worksheets[0].Export(0,0,10,2,true,false);
DataGrid1.SetDataBinding(exportTable, null);
[VB]
Dim exportTable As DataTable =  GridDesktop.Worksheets(0).Export(0,0,10,2,True,False)
DataGrid1.SetDataBinding(exportTable)
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## ExportDataTable(int, int, int, int, GridExportTableOptions) {#exportdatatable}
Exports data in the [`Cells`](../cells/) collection to a DataTable object.
```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns,
GridExportTableOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | The row number of the first cell to export out. |
| firstColumn | Int32 | The column number of the first cell to export out. |
| totalRows | Int32 | Number of rows to be imported. |
| totalColumns | Int32 | Number of columns to be imported. |
| options | GridExportTableOptions | All export table options |
### Return Value
Exported DataTable object.
### See Also
* class [GridExportTableOptions](../../../aspose.cells.griddesktop.data/gridexporttableoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
