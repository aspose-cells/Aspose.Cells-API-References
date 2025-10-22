##ShapeGuideCollection.Add
ShapeGuideCollection method. Adds a shape guide.Important This feature is currently only available for Excel07 and above
## ShapeGuideCollection.Add method
Adds a shape guide.(Important: This feature is currently only available for Excel07 and above)
```csharp
public int Add(string name, double val)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | the name of adjust. It's as "adj(Used when there is only one adjustment value)", "adj1", "adj2", "adj3" and so on. |
| val | Double | the value of adjust |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ShapeGuideCollectionMethodAddWithStringDoubleDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape that uses adjustment guides
Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);
try
{
// Get the ShapeGuideCollection from shape geometry adjustments
ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;
// Call Add method with (String, Double) parameters
shapeGuides.Add("adj1", 25.5);
shapeGuides.Add("adj2", 25.5);
shapeGuides.Add("adj3", 25.5);
shapeGuides.Add("adj4", 25.5);
Console.WriteLine($"Total guides after addition: {shapeGuides.Count}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
// Save the modified workbook
workbook.Save("ShapeGuideAddWithStringDoubleDemo.xlsx");
}
}
}
```
### See Also
* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
