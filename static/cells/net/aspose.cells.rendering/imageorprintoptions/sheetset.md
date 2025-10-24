##ImageOrPrintOptions.SheetSet
ImageOrPrintOptions property. Gets or sets the sheets to render. Default is all visible sheets in the workbook Visible
## ImageOrPrintOptions.SheetSet property
Gets or sets the sheets to render. Default is all visible sheets in the workbook: [`Visible`](../../sheetset/visible/).
```csharp
public SheetSet SheetSet { get; set; }
```
### Remarks
The set is ignored when it is used in [`SheetRender`](../../sheetrender/)
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertySheetSetDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet1 = workbook.Worksheets[0];
sheet1.Name = "VisibleSheet1";
sheet1.Cells["A1"].PutValue("Sheet1 Content");
Worksheet sheet2 = workbook.Worksheets.Add("VisibleSheet2");
sheet2.Cells["A1"].PutValue("Sheet2 Content");
Worksheet sheet3 = workbook.Worksheets.Add("HiddenSheet");
sheet3.Cells["A1"].PutValue("Hidden Content");
sheet3.IsVisible = false;
// Demonstrate SheetSet property with ImageOrPrintOptions
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = ImageType.Tiff;
// Option 1: Print all sheets (including hidden)
options.SheetSet = SheetSet.All;
WorkbookRender allSheetsRender = new WorkbookRender(workbook, options);
Console.WriteLine($"All sheets page count: {allSheetsRender.PageCount}");
// Option 2: Print only visible sheets
options.SheetSet = SheetSet.Visible;
WorkbookRender visibleSheetsRender = new WorkbookRender(workbook, options);
Console.WriteLine($"Visible sheets page count: {visibleSheetsRender.PageCount}");
// Option 3: Print specific sheets by index
options.SheetSet = new SheetSet(new int[] { 0, 2 }); // First and third sheets
WorkbookRender specificSheetsRender = new WorkbookRender(workbook, options);
Console.WriteLine($"Specific sheets page count: {specificSheetsRender.PageCount}");
// Save one page to stream as demonstration
using (MemoryStream stream = new MemoryStream())
{
specificSheetsRender.ToImage(0, stream);
Console.WriteLine($"Image stream length: {stream.Length} bytes");
}
}
}
}
```
### See Also
* class [SheetSet](../../sheetset/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
