##Range.ToImage
Range method. Converts the range to image
## Range.ToImage method
Converts the range to image.
```csharp
public byte[] ToImage(ImageOrPrintOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | ImageOrPrintOptions | The options for converting this range to image |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class RangeMethodToImageWithImageOrPrintOptionsDemo
{
public static void Run()
{
// Create workbook from sample Excel file
Workbook workbook = new Workbook("example.xlsx");
// Get first worksheet and its cells
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create range A1:J25
Aspose.Cells.Range range = cells.CreateRange("A1:J25");
// Create image options
ImageOrPrintOptions options = new ImageOrPrintOptions()
{
ImageType = Aspose.Cells.Drawing.ImageType.Png,
HorizontalResolution = 300,
VerticalResolution = 300
};
// Convert range to image
byte[] imageData = range.ToImage(options);
// Save image to file
File.WriteAllBytes("range_output.png", imageData);
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
