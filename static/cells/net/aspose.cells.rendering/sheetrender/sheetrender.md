##SheetRender.SheetRender
SheetRender constructor. the construct of SheetRender need worksheet and ImageOrPrintOptions as params
## SheetRender constructor
the construct of SheetRender, need worksheet and ImageOrPrintOptions as params
```csharp
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| worksheet | Worksheet | Indicate which spreadsheet to be rendered. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contains some property of output image |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class SheetRenderMethodCtorWithWorksheetImageOrPrintOptionsDemo
{
public static void Run()
{
// Create a workbook and add some sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create image/print options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
options.OnePagePerSheet = true;
// Create SheetRender with Worksheet and ImageOrPrintOptions
SheetRender render = new SheetRender(worksheet, options);
// Output page count
Console.WriteLine("Page count: " + render.PageCount);
// Save the rendered image
render.ToImage(0, "output.png");
}
}
}
```
### See Also
* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
