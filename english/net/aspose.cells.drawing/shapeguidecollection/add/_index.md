---
title: ShapeGuideCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ShapeGuideCollection method. Adds a shape guide.Important This feature is currently only available for Excel07 and above
type: docs
url: /net/aspose.cells.drawing/shapeguidecollection/add/
---
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
namespace AsposeCellsExamples.ShapeGuideCollectionMethodAddWithStringDoubleDemo
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
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 5, 5, 0, 0, 200, 150);

            try
            {
                // Get the ShapeGuideCollection from shape geometry adjustments
                ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

                // Call Add method with (String, Double) parameters
                int guideIndex = shapeGuides.Add("WidthAdjustment", 25.5);

                Console.WriteLine($"Added guide index: {guideIndex}");
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


