##Enum FillPictureType
Aspose.Cells.Drawing.FillPictureType enum. Represents the picture fill type
## FillPictureType enumeration
Represents the picture fill type.
```csharp
public enum FillPictureType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Stretch | `0` | Stretch |
| Stack | `1` | Stack |
| StackAndScale | `2` | StackAndScale |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class DrawingClassFillPictureTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape to demonstrate picture fill
Shape shape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 200, 200);
// Set picture fill properties
shape.Fill.Type = FillType.Texture;
shape.Fill.PictureFormatType = FillPictureType.StackAndScale;
// Use minimal 1x1 pixel image (white) for demonstration
string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
shape.Fill.ImageData = Convert.FromBase64String(base64Image);
// Add another shape with different fill type
Shape shape2 = worksheet.Shapes.AddRectangle(2, 5, 2, 0, 200, 200);
shape2.Fill.Type = FillType.Texture;
shape2.Fill.PictureFormatType = FillPictureType.Stretch;
shape2.Fill.ImageData = Convert.FromBase64String(base64Image);
// Save the workbook with different fill configurations
workbook.Save("FillPictureTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
