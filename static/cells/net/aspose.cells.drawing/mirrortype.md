##Enum MirrorType
Aspose.Cells.Drawing.MirrorType enum. Represents mirror type of texture fill
## MirrorType enumeration
Represents mirror type of texture fill
```csharp
public enum MirrorType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | None |
| Horizonal | `1` | Horizonal |
| Vertical | `2` | Vertical |
| Both | `3` | Both |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class DrawingClassMirrorTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate MirrorType
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 200);
// Set texture fill with different mirror types
shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Horizonal;
shape = worksheet.Shapes.AddRectangle(2, 0, 1, 100, 100, 200);
shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Vertical;
shape = worksheet.Shapes.AddRectangle(3, 0, 1, 100, 100, 200);
shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Both;
shape = worksheet.Shapes.AddRectangle(4, 0, 1, 100, 100, 200);
shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.None;
// Save the result
workbook.Save("MirrorTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
