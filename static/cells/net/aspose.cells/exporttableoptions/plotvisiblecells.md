##ExportTableOptions.PlotVisibleCells
ExportTableOptions property. Only exports visible cells
## ExportTableOptions.PlotVisibleCells property
Only exports visible cells.
```csharp
public bool PlotVisibleCells { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExportTableOptionsPropertyPlotVisibleCellsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with some hidden rows/columns
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["C1"].PutValue("Header3");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["B2"].PutValue("Data2");
worksheet.Cells["C2"].PutValue("Data3");
// Hide row 2 and column B (index 1)
worksheet.Cells.HideRow(1);
worksheet.Cells.HideColumn(1);
// Create export options with PlotVisibleCells set to true
ExportTableOptions exportOptions = new ExportTableOptions
{
PlotVisibleCells = true,
PlotVisibleColumns = true,
PlotVisibleRows = true
};
// Export visible cells only
DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 3, exportOptions);
// Display the exported data (only visible cells should be exported)
Console.WriteLine("Exported Data:");
foreach (DataRow row in dataTable.Rows)
{
foreach (var item in row.ItemArray)
{
Console.Write(item + "\t");
}
Console.WriteLine();
}
}
}
}
```
### See Also
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
