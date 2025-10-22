##PicFormatOption.Top
PicFormatOption property. Gets or sets the top offset for stretching picture
## PicFormatOption.Top property
Gets or sets the top offset for stretching picture.
```csharp
public double Top { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class PicFormatOptionPropertyTopDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Use an existing image or provide correct image path
string imagePath = "existingImage.png";
// Add a shape with correct parameters
Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
// Apply picture fill using ImageData
shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);
// Create and configure PicFormatOption directly
PicFormatOption picFormat = new PicFormatOption();
Console.WriteLine("Initial Top value: " + picFormat.Top);
picFormat.Top = 0.3;
// Assuming PicFormatOption needs to be associated with the fill format
// This part might require API-specific implementation not shown in type definitions
// shape.FillFormat.SetPicFormatOption(picFormat);
Console.WriteLine("Modified Top value: " + picFormat.Top);
workbook.Save("TopPropertyDemo.xlsx");
}
}
}
```
### See Also
* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
