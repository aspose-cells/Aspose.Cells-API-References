##PageSetup.PaperHeight
PageSetup property. Gets the height of the paper in unit of inches  considered page orientation
## PageSetup.PaperHeight property
Gets the height of the paper in unit of inches , considered page orientation.
```csharp
public double PaperHeight { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyPaperHeightDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set some data in a cell
worksheet.Cells["A1"].PutValue("Paper Height Demo");
// Get the PageSetup object
PageSetup pageSetup = worksheet.PageSetup;
// Display default paper height (in inches)
Console.WriteLine("Default Paper Height: " + pageSetup.PaperHeight);
// PaperHeight is read-only, so we demonstrate getting different paper sizes
// by changing the paper size type to Letter (8.5x11 inches)
pageSetup.PaperSize = PaperSizeType.PaperLetter;
// Verify the change
Console.WriteLine("Modified Paper Height (Letter size): " + pageSetup.PaperHeight);
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
