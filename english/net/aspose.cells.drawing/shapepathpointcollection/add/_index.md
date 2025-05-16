---
title: ShapePathPointCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ShapePathPointCollection method. Adds a path point
type: docs
url: /net/aspose.cells.drawing/shapepathpointcollection/add/
---
## ShapePathPointCollection.Add method

Adds a path point.

```csharp
public int Add(int x, int y)
```

| Parameter | Type | Description |
| --- | --- | --- |
| x | Int32 | The x coordinate. |
| y | Int32 | The y coordinate. |

### Examples

```csharp
namespace AsposeCellsExamples.ShapePathPointCollectionMethodAddWithInt32Int32Demo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a shape path point collection
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();

            try
            {
                // Call the Add method with (Int32, Int32) parameters
                int index1 = pathPoints.Add(1000, 2000);
                int index2 = pathPoints.Add(3000, 4000);

                Console.WriteLine($"First point added at index: {index1}");
                Console.WriteLine($"Second point added at index: {index2}");

                // Create a shape path and add the points
                ShapePath path = new ShapePath();
                foreach (ShapePathPoint point in pathPoints)
                {
                    path.LineTo(point.X, point.Y);
                }
                path.Close();

                // Add freeform shape with the configured path
                Shape shape = worksheet.Shapes.AddFreeform(
                    upperLeftRow: 1,
                    top: 1,
                    upperLeftColumn: 0,
                    left: 0,
                    height: 5000,
                    width: 5000,
                    paths: new ShapePath[] { path }
                );

                // Save the result
                workbook.Save("ShapePathPointCollectionMethodAddWithInt32Int32Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [ShapePathPointCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


