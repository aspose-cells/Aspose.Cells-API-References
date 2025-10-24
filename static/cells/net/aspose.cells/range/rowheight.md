##Range.RowHeight
Range property. Sets or gets the height of rows in this range
## Range.RowHeight property
Sets or gets the height of rows in this range
```csharp
public double RowHeight { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyRowHeightDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set some data in the first row
worksheet.Cells["A1"].PutValue("This is a test");
worksheet.Cells["B1"].PutValue("to demonstrate");
worksheet.Cells["C1"].PutValue("RowHeight property");
// Get initial row height
double initialHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
Console.WriteLine("Initial row height: " + initialHeight);
// Auto-fit the row
worksheet.AutoFitRow(0);
// Get the new row height after auto-fit
double newHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
Console.WriteLine("Row height after auto-fit: " + newHeight);
// Manually set a new row height
worksheet.Cells.CreateRange("1:1").RowHeight = 30;
Console.WriteLine("Row height after manual set: " + worksheet.Cells.CreateRange("1:1").RowHeight);
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
