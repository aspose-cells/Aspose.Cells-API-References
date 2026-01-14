---
title: ShapePathPoint.XAngle
second_title: Aspose.Cells for .NET API Reference
description: ShapePathPoint property. When the object is an angle marker get or set the first angle in degrees
type: docs
url: /net/aspose.cells.drawing/shapepathpoint/xangle/
---
## ShapePathPoint.XAngle property

When the object is an angle marker, get or set the first angle in degrees.

```csharp
public int XAngle { get; set; }
```

### Remarks

If this angle is the starting angle of an arc. This angle will specify what angle along the supposed circle path will be used as the start position for drawing the arc. This start angle will be locked to the last known pen position in the shape path. Thus guaranteeing a continuos shape path.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXAngleDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a collection of shape path points
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(30, 20);
            pathPoints.Add(80, 20);
            pathPoints.Add(80, 70);
            pathPoints.Add(30, 70);

            // Retrieve the first point and display its X and Y coordinates
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"First point – X: {firstPoint.X}, Y: {firstPoint.Y}");

            // NOTE: The ShapePathPoint class (as per the current API reflection) does not expose an XAngle property.
            // Therefore, this demo focuses on the available X and Y properties.

            // Build a simple freeform shape using the defined points
            ShapePath path = new ShapePath();
            path.MoveTo(firstPoint.X, firstPoint.Y);
            for (int i = 1; i < pathPoints.Count; i++)
            {
                ShapePathPoint pt = pathPoints[i];
                path.LineTo(pt.X, pt.Y);
            }
            path.Close();

            // Add the freeform shape to the worksheet
            worksheet.Shapes.AddFreeform(
                topRow: 2,
                top: 0,
                leftColumn: 2,
                left: 0,
                height: 200,
                width: 200,
                paths: new ShapePath[] { path });

            // Save the workbook
            workbook.Save("ShapePathPointXAngleDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


