##Shape.IsLockAspectRatio
Shape property. True means that aspect ratio of the shape is locked
## Shape.IsLockAspectRatio property
True means that aspect ratio of the shape is locked.
```csharp
[Obsolete("Use Shape.IsAspectRatioLocked property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsLockAspectRatio { get; set; }
```
### Remarks
Only for pictures and Ole Objects. NOTE: This member is now obsolete. Instead, please use Shape.IsAspectRatioLocked property. This property will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyIsLockAspectRatioDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
// Lock aspect ratio
shape.IsLockAspectRatio = true;
Console.WriteLine("Aspect ratio locked: " + shape.IsLockAspectRatio);
// Unlock aspect ratio
shape.IsLockAspectRatio = false;
Console.WriteLine("Aspect ratio locked: " + shape.IsLockAspectRatio);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
