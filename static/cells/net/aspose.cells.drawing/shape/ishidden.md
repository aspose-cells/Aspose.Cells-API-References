##Shape.IsHidden
Shape property. Indicates whether the object is visible
## Shape.IsHidden property
Indicates whether the object is visible.
```csharp
public bool IsHidden { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyIsHiddenDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
// Set the IsHidden property to false (visible)
shape.IsHidden = false;
Console.WriteLine("Shape is visible: " + !shape.IsHidden);
// Set the IsHidden property to true (hidden)
shape.IsHidden = true;
Console.WriteLine("Shape is hidden: " + shape.IsHidden);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
