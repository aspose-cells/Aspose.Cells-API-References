##Shape.IsLocked
Shape property. True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected
## Shape.IsLocked property
True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.
```csharp
public bool IsLocked { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyIsLockedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);
// Protect the worksheet
worksheet.Protect(ProtectionType.All);
// Demonstrate locking/unlocking the shape
Console.WriteLine("Original IsLocked state: " + shape.IsLocked);
// Unlock the shape
shape.IsLocked = false;
Console.WriteLine("After unlocking, IsLocked state: " + shape.IsLocked);
// Lock the shape
shape.IsLocked = true;
Console.WriteLine("After locking, IsLocked state: " + shape.IsLocked);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
