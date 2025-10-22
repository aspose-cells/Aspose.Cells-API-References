##ImportTableOptions.IsFormulas
ImportTableOptions property. Indicates whether the data are formulas
## ImportTableOptions.IsFormulas property
Indicates whether the data are formulas.
```csharp
public bool[] IsFormulas { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ImportTableOptionsPropertyIsFormulasDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create sample data table with formula content
DataTable dt = new DataTable();
dt.Columns.Add("Column1");
dt.Rows.Add("=SUM(1,2,3)");
dt.Rows.Add("=AVERAGE(4,5,6)");
// Set import options with IsFormulas property
ImportTableOptions options = new ImportTableOptions();
options.IsFormulas = new bool[] { true }; // Treat first column as formulas
// Import data with formulas
workbook.Worksheets[0].Cells.ImportData(dt, 0, 0, options);
// Verify the formulas were imported correctly
Console.WriteLine("Cell A1 formula: " + workbook.Worksheets[0].Cells["A1"].Formula);
Console.WriteLine("Cell A2 formula: " + workbook.Worksheets[0].Cells["A2"].Formula);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
