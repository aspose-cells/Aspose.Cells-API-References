##ImageOrPrintOptions.EmfRenderSetting
ImageOrPrintOptions property. Setting for rendering Emf metafiles in source file
## ImageOrPrintOptions.EmfRenderSetting property
Setting for rendering Emf metafiles in source file.
```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```
### Remarks
EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When EmfPlusPrefer is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed. Default value is EmfOnly. For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
using Aspose.Cells.Rendering;
using System;
public class ImageOrPrintOptionsPropertyEmfRenderSettingDemo
{
public static void Run()
{
// Create a new workbook with test content
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "EMF Rendering Setting Test";
worksheet.Cells["C5"].Value = "Sample Content for Image Rendering";
// Create image rendering options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = ImageType.Tiff;
options.TiffCompression = TiffCompression.CompressionLZW;
// Display current setting
Console.WriteLine("Default EmfRenderSetting: " + options.EmfRenderSetting);
// Render with default EMF settings
SheetRender renderer = new SheetRender(worksheet, options);
renderer.ToImage(0, "DefaultEmfSetting.tiff");
// Change EMF rendering setting and render again
options.EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer;
Console.WriteLine("\nModified EmfRenderSetting: " + options.EmfRenderSetting);
SheetRender modifiedRenderer = new SheetRender(worksheet, options);
modifiedRenderer.ToImage(0, "ModifiedEmfSetting.tiff");
Console.WriteLine("\nGenerated TIFF images demonstrating EMF rendering settings.");
}
}
}
```
### See Also
* enum [EmfRenderSetting](../../../aspose.cells/emfrendersetting/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
