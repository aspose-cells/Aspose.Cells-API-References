##ExportTableOptions.PlotVisibleRows
ExportTableOptions property. Only exports visible rows
## ExportTableOptions.PlotVisibleRows property
Only exports visible rows.
```csharp
public bool PlotVisibleRows { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExportTableOptionsPropertyPlotVisibleRowsDemo
{
public static void Run()
{
// Create a workbook and access the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create sample data in the worksheet
cells["A1"].PutValue("Column1");
cells["A2"].PutValue(10);
cells["A3"].PutValue(20);
cells["A4"].PutValue(30);
// Hide row 3 (index 2) which contains value 20
worksheet.Cells.HideRow(2);
// Create a DataTable to export to
DataTable dataTable = new DataTable();
dataTable.Columns.Add("Column1", typeof(int));
// Set up export options
ExportTableOptions options = new ExportTableOptions();
options.PlotVisibleRows = true; // Only export visible rows
options.ExportColumnName = true;
options.DataTable = dataTable;
// Export data (should skip hidden row)
cells.ExportDataTable(0, 0, 4, 1, options);
// Display the exported data
Console.WriteLine("Exported Data (PlotVisibleRows=true):");
foreach (DataRow row in dataTable.Rows)
{
Console.WriteLine(row["Column1"]);
}
}
}
}
```
### See Also
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
