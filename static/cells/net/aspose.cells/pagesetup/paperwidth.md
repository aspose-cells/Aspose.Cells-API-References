##PageSetup.PaperWidth
PageSetup property. Gets the width of the paper in unit of inches considered page orientation
## PageSetup.PaperWidth property
Gets the width of the paper in unit of inches, considered page orientation.
```csharp
public double PaperWidth { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyPaperWidthDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set some sample data
worksheet.Cells["A1"].PutValue("Sample Page Setup Demo");
// Access the PageSetup of the worksheet
PageSetup pageSetup = worksheet.PageSetup;
// Demonstrate PaperWidth property (read-only)
Console.WriteLine("Paper Width: " + pageSetup.PaperWidth);
// To change paper size, use PaperSize property instead
pageSetup.PaperSize = PaperSizeType.PaperLetter;
Console.WriteLine("New Paper Width: " + pageSetup.PaperWidth);
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
