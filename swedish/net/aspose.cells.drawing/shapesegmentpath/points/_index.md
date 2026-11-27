---
title: "ShapeSegmentPath.Points"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeSegmentPath egenskap. Hämtar punkterna i segmentets bana"
type: docs
url: /sv/net/aspose.cells.drawing/shapesegmentpath/points/
---
## ShapeSegmentPath.Points property

Hämtar punkterna i vägsegmentet

```csharp
public ShapePathPointCollection Points { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathPropertyPointsDemo
    {
        public static void Run()
        {// Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ShapePath path = new ShapePath();

            // Starta en ny sökväg
            path.MoveTo(10, 10);

            // Rita ett linjesegment
            path.LineTo(100, 100);

            // Åtkomst till PathSegementList egenskap
            ShapeSegmentPathCollection segmentPaths = path.PathSegementList;

            // Åtkomst till den första segmentbanan
            ShapeSegmentPath segmentPath = segmentPaths[1];

            // Visa punktinformation
            Console.WriteLine("Number of points in segment: " + segmentPath.Points.Count);
            Console.WriteLine("Point coordinates:");
            foreach (ShapePathPoint point in segmentPath.Points)
            {
                Console.WriteLine($"X: {point.X}, Y: {point.Y}");
            }          

            //lägg till fri form
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

            // Spara arbetsboken
            workbook.Save("ShapeSegmentPathPointsDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapePathPointCollection](../../shapepathpointcollection/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


