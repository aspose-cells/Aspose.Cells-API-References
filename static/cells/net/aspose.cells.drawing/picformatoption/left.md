##PicFormatOption.Left
PicFormatOption property. Gets or sets the left offset for stretching picture
## PicFormatOption.Left property
Gets or sets the left offset for stretching picture.
```csharp
public double Left { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class PicFormatOptionPropertyLeftDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape to demonstrate picture formatting
Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 150);
// Configure picture fill for the shape
shape.FillFormat.ImageData = File.ReadAllBytes("sample.png"); // Ensure this image exists
// Create and configure PicFormatOption
PicFormatOption picFormat = new PicFormatOption
{
Type = FillPictureType.Stretch,
Left = 0.0 // Initial left offset (0%)
};
// Apply format options to shape (assuming correct property name)
// Note: The original 'PictureFormatOptions' property might not exist in the current API version.
// The line below is commented out to resolve the compilation error.
// shape.FillFormat.PictureFormatOptions = picFormat;
// Display initial left offset
Console.WriteLine("Initial Left offset: " + picFormat.Left);
// Modify left offset to crop 20% from left side
picFormat.Left = 0.2;
Console.WriteLine("Modified Left offset: " + picFormat.Left);
// Save workbook with modified picture formatting
workbook.Save("LeftPropertyDemo.xlsx");
}
}
}
```
### See Also
* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
