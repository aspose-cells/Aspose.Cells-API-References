##Range.ColumnWidth
Range property. Sets or gets the column width of this range
## Range.ColumnWidth property
Sets or gets the column width of this range
```csharp
public double ColumnWidth { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class RangePropertyColumnWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access a range (columns B to D)
Aspose.Cells.Range range = worksheet.Cells.CreateRange("B:D");
// Display current column width
Console.WriteLine("Current ColumnWidth: " + range.ColumnWidth);
// Set new column width (in character units)
range.ColumnWidth = 15.0;
// Populate cells to demonstrate the effect
worksheet.Cells["B1"].PutValue("This is column B");
worksheet.Cells["C1"].PutValue("This is column C");
worksheet.Cells["D1"].PutValue("This is column D");
// Auto-fit rows to show content
worksheet.AutoFitRows();
// Save the workbook
workbook.Save("ColumnWidthDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
