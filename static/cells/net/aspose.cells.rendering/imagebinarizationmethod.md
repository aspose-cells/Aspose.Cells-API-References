##Enum ImageBinarizationMethod
Aspose.Cells.Rendering.ImageBinarizationMethod enum. Specifies the method used to binarize image
## ImageBinarizationMethod enumeration
Specifies the method used to binarize image.
```csharp
public enum ImageBinarizationMethod
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Threshold | `0` | Specifies threshold method. |
| FloydSteinbergDithering | `1` | Specifies dithering using Floyd-Steinberg error diffusion method. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;
using System.Drawing;
public class RenderingClassImageBinarizationMethodDemo
{
public static void Run()
{
// Create a new workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate cells with gradient values for demonstration
for (int row = 0; row < 50; row++)
{
for (int col = 0; col < 10; col++)
{
worksheet.Cells[row, col].PutValue((double)(row * col) / 500);
}
}
// Configure image rendering options
ImageOrPrintOptions options = new ImageOrPrintOptions
{
ImageType = ImageType.Tiff,
TiffCompression = TiffCompression.CompressionCCITT4,
TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering
};
// Create sheet render with configured options
SheetRender renderer = new SheetRender(worksheet, options);
// Render first worksheet page to image with binarization
renderer.ToImage(0, "BinarizedOutput.tiff");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
