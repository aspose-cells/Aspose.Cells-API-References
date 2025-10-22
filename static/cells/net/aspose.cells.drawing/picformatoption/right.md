##PicFormatOption.Right
PicFormatOption property. Gets or sets the right offset for stretching picture
## PicFormatOption.Right property
Gets or sets the right offset for stretching picture.
```csharp
public double Right { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class PicFormatOptionPropertyRightDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with specified dimensions
Shape shape = worksheet.Shapes.AddRectangle(5, 2, 10, 10, 150, 300);
// Configure picture fill for the shape
shape.Fill.FillType = FillType.Texture;
string imagePath = "sample.jpg"; // Replace with actual image path
if (File.Exists(imagePath))
{
shape.Fill.ImageData = File.ReadAllBytes(imagePath);
}
else
{
Console.WriteLine("Image not found - using empty picture fill");
}
// Access picture format options through TextureFill
PicFormatOption picFormat = shape.Fill.TextureFill.PicFormatOption;
// Display and modify Right property
Console.WriteLine("Initial Right offset: " + picFormat.Right);
picFormat.Right = 25.5; // Set right offset to 25.5 units
// Verify new value and save changes
Console.WriteLine("Updated Right offset: " + picFormat.Right);
workbook.Save("RightPropertyDemo.xlsx");
}
}
}
```
### See Also
* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
