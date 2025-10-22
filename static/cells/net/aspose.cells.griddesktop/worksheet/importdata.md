##Worksheet.ImportData
Worksheet method. Import data from custom data table
## Worksheet.ImportData method
Import data from custom data table.
```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn,
GridImportTableOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| table | DataTable | The DataTable object to be imported. |
| firstRow | Int32 | First row index. |
| firstColumn | Int32 | First column index. |
| options | GridImportTableOptions | The import options |
### Return Value
Total number of rows imported.
### Examples
```csharp
[C#]
Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;
//Import data
DataTable dt = new DataTable("Products");
dt.Columns.Add("Product_ID",typeof(Int32));
dt.Columns.Add("Product_Name",typeof(string));
dt.Columns.Add("Units_In_Stock",typeof(Int32));
DataRow dr = dt.NewRow();
dr[0] = 1;
dr[1] = "Aniseed Syrup";
dr[2] = 15;
dt.Rows.Add(dr);
dr = dt.NewRow();
dr[0] = 2;
dr[1] = "Boston Crab Meat";
dr[2] = 123;
dt.Rows.Add(dr);
ImportTableOptions options = new ImportTableOptions();
options.IsFieldNameShown = true;
cells.ImportData(dt, 12, 12, options);
[Visual Basic]
Dim excel as Workbook = new Workbook()
Dim cells as Cells = excel.Worksheets(0).Cells
'Import data
Dim dt as DataTable = new DataTable("Employee")
dt.Columns.Add("Employee_ID",typeof(Int32))
dt.Columns.Add("Employee_Name",typeof(string))
dt.Columns.Add("Gender",typeof(string))
Dim dr as DataRow = dt.NewRow()
dr(0) = 1
dr(1) = "John Smith"
dr(2) = "Male"
dt.Rows.Add(dr)
dr = dt.NewRow()
dr(0) = 2
dr(1) = "Mary Miller"
dr(2) = "Female"
dt.Rows.Add(dr)
Dim options as ImportTableOptions = new ImportTableOptions()
options.IsFieldNameShown = True
cells.ImportData(dt, 12, 12, options)
'Export data
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```
### See Also
* class [GridImportTableOptions](../../../aspose.cells.griddesktop.data/gridimporttableoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
