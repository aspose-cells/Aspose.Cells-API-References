##ExportTableOptions.PlotVisibleColumns
ExportTableOptions property. Only exports visible columns
## ExportTableOptions.PlotVisibleColumns property
Only exports visible columns.
```csharp
public bool PlotVisibleColumns { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExportTableOptionsPropertyPlotVisibleColumnsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and hide some columns
worksheet.Cells["A1"].PutValue("Column1");
worksheet.Cells["B1"].PutValue("Column2");
worksheet.Cells["C1"].PutValue("Column3");
worksheet.Cells["D1"].PutValue("Column4");
for (int i = 2; i <= 5; i++)
{
worksheet.Cells[$"A{i}"].PutValue($"Data{i-1}_1");
worksheet.Cells[$"B{i}"].PutValue($"Data{i-1}_2");
worksheet.Cells[$"C{i}"].PutValue($"Data{i-1}_3");
worksheet.Cells[$"D{i}"].PutValue($"Data{i-1}_4");
}
// Hide column C
worksheet.Cells.HideColumn(2);
// Export data with PlotVisibleColumns set to true
ExportTableOptions options = new ExportTableOptions();
options.ExportColumnName = true;
options.PlotVisibleColumns = true;
DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 6, 4, options);
// Output the results
Console.WriteLine("Exported DataTable Columns:");
foreach (DataColumn column in dataTable.Columns)
{
Console.WriteLine(column.ColumnName);
}
}
}
}
```
### See Also
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
