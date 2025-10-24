##AutoFitterOptions.IgnoreHidden
AutoFitterOptions property. Ignores the hidden rows/columns
## AutoFitterOptions.IgnoreHidden property
Ignores the hidden rows/columns.
```csharp
public bool IgnoreHidden { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFitterOptionsPropertyIgnoreHiddenDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data and format rows
worksheet.Cells["A1"].PutValue("This is a test string for autofit");
worksheet.Cells["A2"].PutValue("Another test string");
// Hide row 1
worksheet.Cells.Rows[1].IsHidden = true;
// Create AutoFitterOptions with IgnoreHidden set to true
AutoFitterOptions options = new AutoFitterOptions
{
IgnoreHidden = true,
AutoFitMergedCells = false,
OnlyAuto = false
};
// Autofit rows while ignoring hidden rows
worksheet.AutoFitRows(options);
// Output the row heights
Console.WriteLine("Row 0 height: " + worksheet.Cells.GetRowHeight(0));
Console.WriteLine("Row 1 height: " + worksheet.Cells.GetRowHeight(1));
}
}
}
```
### See Also
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
