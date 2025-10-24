##Shape.LineFormat
Shape property. Returns a MsoLineFormat object that contains line formatting properties for the specified shape
## Shape.LineFormat property
Returns a MsoLineFormat object that contains line formatting properties for the specified shape.
```csharp
[Obsolete("Use Shape.Line property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoLineFormat LineFormat { get; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.Line property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyLineFormatDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a rectangle shape to the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
RectangleShape rectangle = worksheet.Shapes.AddRectangle(3, 0, 2, 0, 70, 130);
// Set shape properties
rectangle.Placement = PlacementType.FreeFloating;
rectangle.Fill.FillType = FillType.Solid;
rectangle.Fill.SolidFill.Color = System.Drawing.Color.Blue;
// Demonstrate LineFormat usage
rectangle.LineFormat.Weight = 3; // Set line weight
rectangle.LineFormat.DashStyle = MsoLineDashStyle.Solid;
rectangle.Line.SolidFill.Color = System.Drawing.Color.DarkBlue; // Correct way to set line color
// Save the workbook
workbook.Save("ShapeLineFormatDemo.xlsx");
}
}
}
```
### See Also
* class [MsoLineFormat](../../msolineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
