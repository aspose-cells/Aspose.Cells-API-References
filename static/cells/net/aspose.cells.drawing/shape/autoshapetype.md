##Shape.AutoShapeType
Shape property. Gets and sets the auto shape type
## Shape.AutoShapeType property
Gets and sets the auto shape type.
```csharp
public AutoShapeType AutoShapeType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyAutoShapeTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet with correct parameters
Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 100, 150, 0, 0);
// Check and modify the AutoShapeType if needed
if (shape.AutoShapeType == AutoShapeType.Unknown)
{
shape.AutoShapeType = AutoShapeType.Rectangle;
}
// Change the shape type to demonstrate the property
shape.AutoShapeType = AutoShapeType.Oval;
// Save the workbook
workbook.Save("ShapePropertyAutoShapeTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
