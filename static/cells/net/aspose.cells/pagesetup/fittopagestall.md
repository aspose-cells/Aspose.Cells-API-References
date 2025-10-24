##PageSetup.FitToPagesTall
PageSetup property. Represents the number of pages tall the worksheet will be scaled to when its printed. The default value is 1
## PageSetup.FitToPagesTall property
Represents the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1.
```csharp
public int FitToPagesTall { get; set; }
```
### Remarks
You have to set FitToPagesWide as zero if you want to fit all rows on one page.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PageSetupPropertyFitToPagesTallDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to make the sheet span multiple pages
for (int i = 0; i < 100; i++)
{
for (int j = 0; j < 10; j++)
{
worksheet.Cells[i, j].PutValue($"Row {i+1}, Col {j+1}");
}
}
// Get PageSetup object
PageSetup pageSetup = worksheet.PageSetup;
// Set print area
pageSetup.PrintArea = "A1:J100";
// Set FitToPagesTall property to fit all rows on one page
pageSetup.FitToPagesTall = 1;
// Set FitToPagesWide property to fit all columns on one page
pageSetup.FitToPagesWide = 1;
// Set paper size
pageSetup.PaperSize = PaperSizeType.PaperLetter;
// Print gridlines
pageSetup.PrintGridlines = true;
// Create rendering options
ImageOrPrintOptions options = new ImageOrPrintOptions();
// Create sheet renderer
SheetRender render = new SheetRender(worksheet, options);
// Output the page scale
Console.WriteLine($"Page scale: {Math.Round(render.PageScale, 2)}");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
