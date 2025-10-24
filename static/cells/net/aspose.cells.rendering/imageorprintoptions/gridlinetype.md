##ImageOrPrintOptions.GridlineType
ImageOrPrintOptions property. Gets or sets gridline type
## ImageOrPrintOptions.GridlineType property
Gets or sets gridline type.
```csharp
public GridlineType GridlineType { get; set; }
```
### Remarks
Default is Dotted type.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;
using System;
public class ImageOrPrintOptionsPropertyGridlineTypeDemo
{
public static void Run()
{
// Create a new workbook and populate sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Book");
worksheet.Cells["B2"].PutValue("$19.99");
worksheet.Cells["A3"].PutValue("Pen");
worksheet.Cells["B3"].PutValue("$2.99");
// Create ImageOrPrintOptions instance
ImageOrPrintOptions imageOptions = new ImageOrPrintOptions
{
ImageType = ImageType.Png,
GridlineType = GridlineType.Dotted // Use valid enum value
};
// Display current gridline type
Console.WriteLine("Initial GridlineType: " + imageOptions.GridlineType);
// Render worksheet with initial gridline type
SheetRender solidLineRenderer = new SheetRender(worksheet, imageOptions);
solidLineRenderer.ToImage(0, "SolidGridlines.png");
// Change gridline type and render again
imageOptions.GridlineType = GridlineType.Hair; // Use valid enum value
Console.WriteLine("\nModified GridlineType: " + imageOptions.GridlineType);
SheetRender dashedLineRenderer = new SheetRender(worksheet, imageOptions);
dashedLineRenderer.ToImage(0, "DashedGridlines.png");
Console.WriteLine("Generated images demonstrate different gridline styles.");
}
}
}
```
### See Also
* enum [GridlineType](../../../aspose.cells/gridlinetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
