##Shape.RelativeToOriginalPictureSize
Shape property. Indicates whether shape is relative to original picture size
## Shape.RelativeToOriginalPictureSize property
Indicates whether shape is relative to original picture size.
```csharp
public bool RelativeToOriginalPictureSize { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyRelativeToOriginalPictureSizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int index = worksheet.Pictures.Add(0, 0, "example.jpg");
Picture picture = worksheet.Pictures[index];
// Access the shape properties - Picture is already a Shape, no need to cast
Shape shape = picture;
// Demonstrate RelativeToOriginalPictureSize property
Console.WriteLine("Original RelativeToOriginalPictureSize: " + shape.RelativeToOriginalPictureSize);
// Change the property
shape.RelativeToOriginalPictureSize = !shape.RelativeToOriginalPictureSize;
Console.WriteLine("Modified RelativeToOriginalPictureSize: " + shape.RelativeToOriginalPictureSize);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
