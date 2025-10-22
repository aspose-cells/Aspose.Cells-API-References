##ShapeGuide.Value
ShapeGuide property. Gets or sets value of this guide
## ShapeGuide.Value property
Gets or sets value of this guide
```csharp
public double Value { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ShapeGuidePropertyValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape that uses adjustment guides
Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);
// Access the shape's adjustment guides collection via Geometry
ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;
// Add new guides to the collection
shapeGuides.Add("adj1", 25.5);
shapeGuides.Add("adj2", 30);
shapeGuides.Add("adj3", 25.5);
shapeGuides.Add("adj4", 35);
// Demonstrate reading guide values (Name property not available in provided definition)
Console.WriteLine("First guide value: " + shapeGuides[0].Value);
Console.WriteLine("Second guide value: " + shapeGuides[1].Value);
Console.WriteLine("third guide value: " + shapeGuides[2].Value);
Console.WriteLine("fourth guide value: " + shapeGuides[3].Value);
Console.WriteLine("Updated adjustment values");
shapeGuides[0].Value = 25.5;
shapeGuides[1].Value = 25.5;
shapeGuides[2].Value = 25.5;
shapeGuides[3].Value = 25.5;
Console.WriteLine("First guide value: " + shapeGuides[0].Value);
Console.WriteLine("Second guide value: " + shapeGuides[1].Value);
Console.WriteLine("third guide value: " + shapeGuides[2].Value);
Console.WriteLine("fourth guide value: " + shapeGuides[3].Value);
// Save the modified workbook
workbook.Save("ShapeGuideValueDemo.xlsx");
}
}
}
```
### See Also
* class [ShapeGuide](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
