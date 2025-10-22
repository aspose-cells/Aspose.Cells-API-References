##ImageOrPrintOptions.SVGFitToViewPort
ImageOrPrintOptions property. if this property is true the generated svg will fit to view port
## ImageOrPrintOptions.SVGFitToViewPort property
if this property is true, the generated svg will fit to view port.
```csharp
[Obsolete("Use SvgImageOptions.FitToViewPort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SVGFitToViewPort { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use [`FitToViewPort`](../../svgimageoptions/fittoviewport/). This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertySVGFitToViewPortDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["B1"].PutValue("Quantity");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(15);
// Create image options for SVG output
ImageOrPrintOptions opts = new ImageOrPrintOptions();
opts.ImageType = Aspose.Cells.Drawing.ImageType.Svg;
opts.OnePagePerSheet = true;
opts.SVGFitToViewPort = true; // This is the key property being demonstrated
// Render the worksheet to SVG image
SheetRender sr = new SheetRender(worksheet, opts);
sr.ToImage(0, "output.svg");
Console.WriteLine("SVG file with SVGFitToViewPort=true created successfully.");
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
