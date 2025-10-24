##ImageOrPrintOptions.Quality
ImageOrPrintOptions property. Gets or sets a value determining the quality of the generated images to apply only when saving pages to the Jpeg format. The default value is 100
## ImageOrPrintOptions.Quality property
Gets or sets a value determining the quality of the generated images to apply only when saving pages to the `Jpeg` format. The default value is 100
```csharp
public int Quality { get; set; }
```
### Remarks
Has effect only when saving to JPEG. The value must be between 0 and 100. The default value is 100.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyQualityDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Sample Text");
worksheet.Cells["B2"].PutValue(123.45);
worksheet.Cells["C3"].PutValue(DateTime.Now);
// Create image options with different quality settings
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;
options.Quality = 100; // Highest quality
// Render worksheet to image with high quality
SheetRender renderer = new SheetRender(worksheet, options);
renderer.ToImage(0, "HighQualityOutput.jpg");
// Change quality to demonstrate difference
options.Quality = 50; // Medium quality
renderer.ToImage(0, "MediumQualityOutput.jpg");
options.Quality = 10; // Low quality
renderer.ToImage(0, "LowQualityOutput.jpg");
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
