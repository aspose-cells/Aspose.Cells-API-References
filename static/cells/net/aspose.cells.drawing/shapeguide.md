##Class ShapeGuide
Aspose.Cells.Drawing.ShapeGuide class. Encapsulates a shape guide specifies the presence of a shape guide that will be used to govern the geometry of the specified shape
## ShapeGuide class
Encapsulates a shape guide specifies the presence of a shape guide that will be used to govern the geometry of the specified shape
```csharp
public class ShapeGuide : BaseShapeGuide
```
## Properties
| Name | Description |
| --- | --- |
| [Value](../../aspose.cells.drawing/shapeguide/value/) { get; set; } | Gets or sets value of this guide |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class DrawingClassShapeGuideDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 0, 0, 100, 100, 100, 100);
// Create and add shape guide with required parameters
int guideIndex = shape.Geometry.ShapeAdjustValues.Add("Guide1", 0.2);
ShapeGuide guide = shape.Geometry.ShapeAdjustValues[guideIndex];
Console.WriteLine($"ShapeGuide created with Value: {guide.Value}");
workbook.Save("DrawingClassShapeGuideDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [BaseShapeGuide](../baseshapeguide/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
