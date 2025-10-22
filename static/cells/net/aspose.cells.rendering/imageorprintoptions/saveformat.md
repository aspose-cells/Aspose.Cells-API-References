##ImageOrPrintOptions.SaveFormat
ImageOrPrintOptions property. Gets or sets the output file format type Support Tiff/XPS
## ImageOrPrintOptions.SaveFormat property
Gets or sets the output file format type Support Tiff/XPS
```csharp
[Obsolete("For Tiff/Svg, use ImageType; For Xps, use Workbook.Save(string, SaveOptions) with XpsSaveOptions")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SaveFormat SaveFormat { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, For Tiff/Svg, use [`ImageType`](../imagetype/); For Xps, use [`Save`](../../../aspose.cells/workbook/save/) with [`XpsSaveOptions`](../../../aspose.cells/xpssaveoptions/). This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
using System.IO;
public class ImageOrPrintOptionsPropertySaveFormatDemo
{
public static void Run()
{
// Create a new workbook and populate sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Aspose.Cells SaveFormat Demonstration");
// Create ImageOrPrintOptions instance
ImageOrPrintOptions options = new ImageOrPrintOptions();
// Display initial SaveFormat value
Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);
// Set SaveFormat to TIFF and render worksheet
options.SaveFormat = SaveFormat.Tiff;
SheetRender tiffRenderer = new SheetRender(worksheet, options);
using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
{
tiffRenderer.ToTiff(tiffStream);
}
Console.WriteLine("Rendered worksheet to TIFF format");
// Change SaveFormat to XPS and render again
options.SaveFormat = SaveFormat.Xps;
SheetRender xpsRenderer = new SheetRender(worksheet, options);
using (FileStream xpsStream = new FileStream("output.xps", FileMode.Create))
{
// Note: SheetRender does not support XPS format. This will save as image format instead.
xpsRenderer.ToImage(0, xpsStream);
}
Console.WriteLine("Rendered worksheet to XPS format");
}
}
}
```
### See Also
* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
