##Cells.StandardHeightPixels
Cells property. Gets or sets the default row height in this worksheet in unit of pixels
## Cells.StandardHeightPixels property
Gets or sets the default row height in this worksheet, in unit of pixels.
```csharp
public int StandardHeightPixels { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyStandardHeightPixelsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set some data in cells
cells["A1"].PutValue("Sample Data");
cells["B2"].PutValue(123);
cells["C3"].PutValue(DateTime.Now);
// Get the standard height in pixels
int standardHeight = cells.StandardHeightPixels;
Console.WriteLine("Standard row height in pixels: " + standardHeight);
// Display row heights (should match standard height)
for (int i = 0; i < 5; i++)
{
int rowHeight = cells.GetRowHeightPixel(i);
Console.WriteLine($"Row {i} height: {rowHeight}px");
Console.WriteLine($"Matches standard: {rowHeight == standardHeight}");
}
// Change standard height and verify
cells.StandardHeight = 20; // Set in points
int newStandardHeight = cells.StandardHeightPixels;
Console.WriteLine("\nNew standard height in pixels: " + newStandardHeight);
// Verify all rows now have the new height
for (int i = 0; i < 5; i++)
{
int rowHeight = cells.GetRowHeightPixel(i);
Console.WriteLine($"Row {i} height: {rowHeight}px");
Console.WriteLine($"Matches new standard: {rowHeight == newStandardHeight}");
}
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
