##TilePicOption.MirrorType
TilePicOption property. Gets or sets the mirror type for tiling
## TilePicOption.MirrorType property
Gets or sets the mirror type for tiling.
```csharp
public MirrorType MirrorType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class TilePicOptionPropertyMirrorTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 500, 500, 500);
// Load sample image data (replace with actual image path)
byte[] imageData = File.ReadAllBytes("sample.png");
// Create and configure TilePicOption instance
TilePicOption tileOptions = new TilePicOption();
// Display initial MirrorType value
Console.WriteLine("Current MirrorType: " + tileOptions.MirrorType);
// Configure tiling options
tileOptions.ScaleX = 0.5;
tileOptions.ScaleY = 0.5;
tileOptions.MirrorType = MirrorType.Both;
// Apply tile configuration using correct properties
shape.Fill.FillType = FillType.Texture;
shape.Fill.ImageData = imageData;
shape.Fill.TextureFill.TilePicOption = tileOptions;
// Save the modified workbook
workbook.Save("TilePicOptionMirrorTypeDemo.xlsx");
Console.WriteLine("Updated MirrorType: " + tileOptions.MirrorType);
}
}
}
```
### See Also
* enum [MirrorType](../../mirrortype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
