##Shape.Line
Shape property. Gets line style
## Shape.Line property
Gets line style
```csharp
public LineFormat Line { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyLineDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape (returns LineShape directly)
LineShape lineShape = worksheet.Shapes.AddLine(1, 0, 1, 0, 5, 100);
// Access and modify line properties
LineFormat lineFormat = lineShape.Line;
lineFormat.CompoundType = MsoLineStyle.ThickThin;
lineFormat.DashStyle = MsoLineDashStyle.DashDot;
lineFormat.Weight = 3.0;
lineFormat.BeginArrowheadStyle = MsoArrowheadStyle.Arrow;
lineFormat.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;
// Save the workbook
workbook.Save("LineShapeDemo.xlsx");
}
}
}
```
### See Also
* class [LineFormat](../../lineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
