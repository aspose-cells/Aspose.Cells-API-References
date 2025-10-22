##LowCodeImageSaveOptions.SaveFormat
LowCodeImageSaveOptions property. Gets or sets the save format
## LowCodeImageSaveOptions.SaveFormat property
Gets or sets the save format.
```csharp
public override SaveFormat SaveFormat { get; set; }
```
### Remarks
If [`ImageOptions`](../imageoptions/) has been specified, setting this property will also change the [`ImageType`](../../../aspose.cells.rendering/imageorprintoptions/imagetype/) value of it.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.LowCode;
using Aspose.Cells.Rendering;
using System;
public class LowCodeImageSaveOptionsPropertySaveFormatDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Aspose.Cells LowCode Image SaveFormat Demo");
// Initialize LowCodeImageSaveOptions with default values
LowCodeImageSaveOptions options = new LowCodeImageSaveOptions();
// Display initial SaveFormat (default is Png)
Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);
// Configure for JPEG output
options.SaveFormat = SaveFormat.Jpg;
options.ImageOptions = new ImageOrPrintOptions
{
Quality = 85,
OnePagePerSheet = true,
ImageType = ImageType.Jpeg
};
SaveWorksheetAsImage(worksheet, options, "output_initial.jpg");
// Change to PNG format and save again
options.SaveFormat = SaveFormat.Png;
options.ImageOptions.ImageType = ImageType.Png;
Console.WriteLine("\nModified SaveFormat: " + options.SaveFormat);
SaveWorksheetAsImage(worksheet, options, "output_modified.png");
}
private static void SaveWorksheetAsImage(Worksheet worksheet, LowCodeImageSaveOptions options, string fileName)
{
// Render worksheet using configured options
SheetRender renderer = new SheetRender(worksheet, options.ImageOptions);
renderer.ToImage(0, fileName);
Console.WriteLine($"Saved: {fileName}");
}
}
}
```
### See Also
* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
