##TilePicOption.AlignmentType
TilePicOption property. Gets or sets the alignment for tiling
## TilePicOption.AlignmentType property
Gets or sets the alignment for tiling.
```csharp
public RectangleAlignmentType AlignmentType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class TilePicOptionPropertyAlignmentTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape to demonstrate tiling
Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 300);
// Configure fill format to use tiled picture
FillFormat fillFormat = rectangle.Fill;
fillFormat.FillType = FillType.Texture;
// Create and configure TilePicOption
TilePicOption tileOptions = new TilePicOption();
// Display initial AlignmentType value
Console.WriteLine("Current AlignmentType: " + tileOptions.AlignmentType);
// Set alignment to TopRight
tileOptions.AlignmentType = RectangleAlignmentType.TopRight;
tileOptions.ScaleX = 0.5;
tileOptions.ScaleY = 0.5;
// Apply tile options to shape fill
fillFormat.TextureFill.TilePicOption = tileOptions;
// Load sample image (1x1 pixel red dot)
byte[] imageData = Convert.FromBase64String(
"iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
fillFormat.ImageData = imageData;
// Save modified workbook
workbook.Save("TilePicOptionPropertyAlignmentTypeDemo.xlsx");
// Change alignment to BottomLeft and save another version
tileOptions.AlignmentType = RectangleAlignmentType.BottomLeft;
workbook.Save("TilePicOptionPropertyAlignmentTypeDemo_BottomLeft.xlsx");
}
}
}
```
### See Also
* enum [RectangleAlignmentType](../../rectanglealignmenttype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
