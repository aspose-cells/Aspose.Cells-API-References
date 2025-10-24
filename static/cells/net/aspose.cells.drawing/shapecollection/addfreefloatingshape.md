##ShapeCollection.AddFreeFloatingShape
ShapeCollection method. Adds a free floating shape to the worksheet.Only applies for line/image shape
## ShapeCollection.AddFreeFloatingShape method
Adds a free floating shape to the worksheet.Only applies for line/image shape.
```csharp
public Shape AddFreeFloatingShape(MsoDrawingType type, int top, int left, int height, int width,
byte[] imageData, bool isOriginalSize)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | The shape type. |
| top | Int32 | Represents the vertical offset of shape from the worksheet's top row, in unit of pixel. |
| left | Int32 | Represents the horizontal offset of shape from the worksheet's left column, in unit of pixel. |
| height | Int32 | Represents the height of LineShape, in unit of pixel. |
| width | Int32 | Represents the width of LineShape, in unit of pixel. |
| imageData | Byte[] | The image data,only applies for the picture. |
| isOriginalSize | Boolean | Whether the shape use original size if the shape is image. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodAddFreeFloatingShapeWithMsoDrawingTypeInt32Int32Int32IDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ShapeCollection shapes = worksheet.Shapes;
// Add a line shape
Shape floatingShape_Line = shapes.AddFreeFloatingShape(
MsoDrawingType.Line,
100, 100, 100, 50,
null,
false);
// Add a picture shape (using sample image data)
byte[] imageData = null;
try
{
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
imageData = new byte[fs.Length];
fs.Read(imageData, 0, (int)fs.Length);
}
}
catch
{
// Create dummy image data if file not found
imageData = new byte[100];
}
Shape floatingShape_Picture = shapes.AddFreeFloatingShape(
MsoDrawingType.Picture,
200, 100, 100, 50,
imageData,
false);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
