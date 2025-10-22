##ImageSaveOptions.ImageSaveOptions
ImageSaveOptions constructor. Creates the options for saving image file
## ImageSaveOptions() {#constructor}
Creates the options for saving image file.
```csharp
public ImageSaveOptions()
```
### Remarks
The default type is Tiff.
### See Also
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ImageSaveOptions(SaveFormat) {#constructor_1}
Creates the options for saving image file.
```csharp
public ImageSaveOptions(SaveFormat saveFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be one of following types: Tiff, Svg, Bmp, Png, Jpg, Emf or Gif, otherwise the saved format will be set as Tiff automatically. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class ImageSaveOptionsMethodCtorWithSaveFormatDemo
{
public static void Run()
{
// Create a new workbook and add test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Aspose.Cells Image Save Demo");
// Create ImageSaveOptions with SaveFormat.Tiff
try
{
ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Tiff);
// Configure image rendering options
saveOptions.ImageOrPrintOptions.HorizontalResolution = 300;
saveOptions.ImageOrPrintOptions.VerticalResolution = 300;
// Save workbook as multi-page TIFF
workbook.Save("WorksheetImage.tiff", saveOptions);
Console.WriteLine("Workbook successfully saved as TIFF image with 300 DPI resolution.");
}
catch (Exception ex)
{
Console.WriteLine($"Error during image save operation: {ex.Message}");
}
}
}
}
```
### See Also
* enum [SaveFormat](../../saveformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
