##SheetRender.PageCount
SheetRender property. Gets the total page count of current worksheet
## SheetRender.PageCount property
Gets the total page count of current worksheet.
```csharp
public int PageCount { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class SheetRenderPropertyPageCountDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
Cells cells = worksheet.Cells;
cells["A1"].PutValue("Name");
cells["B1"].PutValue("Age");
cells["A2"].PutValue("John");
cells["B2"].PutValue(30);
cells["A3"].PutValue("Mary");
cells["B3"].PutValue(25);
cells["A4"].PutValue("Peter");
cells["B4"].PutValue(35);
// Set page setup for printing
PageSetup pageSetup = worksheet.PageSetup;
pageSetup.PrintArea = "A1:B4";
pageSetup.FitToPagesTall = 1;
pageSetup.FitToPagesWide = 1;
// Create SheetRender with default options
ImageOrPrintOptions options = new ImageOrPrintOptions();
SheetRender render = new SheetRender(worksheet, options);
// Display the page count
Console.WriteLine("Page Count: " + render.PageCount);
// Change page setup to force multiple pages
pageSetup.FitToPagesTall = 0;
pageSetup.FitToPagesWide = 1;
pageSetup.PrintArea = "A1:B100"; // Larger area than can fit on one page
// Create new SheetRender to get updated page count
SheetRender newRender = new SheetRender(worksheet, options);
Console.WriteLine("Updated Page Count: " + newRender.PageCount);
}
}
}
```
### See Also
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
