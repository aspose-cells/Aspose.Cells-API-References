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
namespace AsposeCellsExamples
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
                pathPoints.Add(50, 10);
                pathPoints.Add(50, 50);
                pathPoints.Add(10, 50);

                // Create a shape path and add the points
                ShapePath path = new ShapePath();

                // Move to starting point
                path.MoveTo(10, 10);

                foreach (ShapePathPoint point in pathPoints)
                {
                    path.LineTo(point.X, point.Y);
                }
                path.Close();

                // Add freeform shape with the configured path
                Shape shape = worksheet.Shapes.AddFreeform(
                    upperLeftRow: 2,
                    top: 0,
                    upperLeftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
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


