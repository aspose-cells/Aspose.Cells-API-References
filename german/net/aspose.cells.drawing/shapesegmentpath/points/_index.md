---
title: "ShapeSegmentPath.Points"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeSegmentPath-Eigenschaft. Gibt die Punkte im Pfadsegment zurück"
type: docs
url: /de/net/aspose.cells.drawing/shapesegmentpath/points/
---
## ShapeSegmentPath.Points property

Ermittelt die Punkte im Pfadsegment

```csharp
public ShapePathPointCollection Points { get; }
```

### Beispiele

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

            // Beginnen Sie einen neuen Pfad
            path.MoveTo(10, 10);

            // Zeichne ein Liniensegment
            path.LineTo(100, 100);

            // Greifen Sie auf die PathSegementList-Eigenschaft zu
            ShapeSegmentPathCollection segmentPaths = path.PathSegementList;

            // Greifen Sie auf den ersten Segmentpfad zu
            ShapeSegmentPath segmentPath = segmentPaths[1];

            // Punktinformationen anzeigen
            Console.WriteLine("Number of points in segment: " + segmentPath.Points.Count);
            Console.WriteLine("Point coordinates:");
            foreach (ShapePathPoint point in segmentPath.Points)
            {
                Console.WriteLine($"X: {point.X}, Y: {point.Y}");
            }          

            //Freiform hinzufügen
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeSegmentPathPointsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapePathPointCollection](../../shapepathpointcollection/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


