##PicFormatOption.Bottom
PicFormatOption property. Gets or sets the bottom offset for stretching picture
## PicFormatOption.Bottom property
Gets or sets the bottom offset for stretching picture.
```csharp
public double Bottom { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class PicFormatOptionPropertyBottomDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Use an existing image file (replace with actual image path)
string imagePath = "sample.jpg";
// Add a rectangle shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);
// Configure shape fill to use the sample image
// FillType is inferred by setting ImageData, which sets the type to Texture
shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);
// Create and configure the picture format options
PicFormatOption picFormat = new PicFormatOption();
picFormat.Type = FillPictureType.Stretch;
// Display initial Bottom value
Console.WriteLine("Initial Bottom value: " + picFormat.Bottom);
// Modify the Bottom offset and display new value
picFormat.Bottom = 0.3;
Console.WriteLine("Modified Bottom value: " + picFormat.Bottom);
// Associate the PicFormatOption with the shape's fill (assuming applicable)
// Note: This step may require API-specific methods not shown in the provided context
// For demonstration, the PicFormatOption is created and configured
// Save the workbook with applied changes
workbook.Save("PicFormatOptionBottomDemo.xlsx");
}
}
}
```
### See Also
* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
