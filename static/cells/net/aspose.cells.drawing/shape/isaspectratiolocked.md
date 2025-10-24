##Shape.IsAspectRatioLocked
Shape property. True means that aspect ratio of the shape is locked
## Shape.IsAspectRatioLocked property
True means that aspect ratio of the shape is locked.
```csharp
public bool IsAspectRatioLocked { get; set; }
```
### Remarks
Only for pictures and Ole Objects.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyIsAspectRatioLockedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 50);
Console.WriteLine("Original Aspect Ratio Locked: " + shape.IsAspectRatioLocked);
shape.IsAspectRatioLocked = true;
Console.WriteLine("After setting to true: " + shape.IsAspectRatioLocked);
shape.IsAspectRatioLocked = false;
Console.WriteLine("After setting to false: " + shape.IsAspectRatioLocked);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
