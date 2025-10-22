##TilePicOption.OffsetX
TilePicOption property. Gets or sets the X offset for tiling picture
## TilePicOption.OffsetX property
Gets or sets the X offset for tiling picture.
```csharp
public double OffsetX { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class TilePicOptionPropertyOffsetXDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape to demonstrate tiling
Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
// Configure fill format to use tiled picture
FillFormat fillFormat = rectangle.Fill;
fillFormat.FillType = FillType.Texture;
// Create and configure TilePicOption
TilePicOption tileOptions = new TilePicOption();
// Read initial OffsetX value
Console.WriteLine("Current OffsetX value: " + tileOptions.OffsetX);
// Set new X offset for tiling pattern
tileOptions.OffsetX = 15.5;
// Apply tile options to shape fill
fillFormat.TextureFill.TilePicOption = tileOptions;
// Load minimal 1x1 pixel image (red dot)
byte[] imageData = Convert.FromBase64String(
"iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
fillFormat.ImageData = imageData;
// Save modified workbook
workbook.Save("TilePicOptionPropertyOffsetXDemo.xlsx");
}
}
}
```
### See Also
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
