---
title: "ShapePathPointCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePathPointCollection‑egenskap. Hämtar shape path point efter index"
type: docs
url: /sv/net/aspose.cells.drawing/shapepathpointcollection/item/
---
## ShapePathPointCollection indexer

Hämtar formbanpunkt efter index.

```csharp
public ShapePathPoint this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet |

### Returvärde

Returnerar [`ShapePathPoint`](../../shapepathpoint/)-objekt

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en shape path point‑samling och lägg till punkter
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(50, 10);
            pathPoints.Add(50, 50);
            pathPoints.Add(10, 50);

            // Åtkomst till punkter med Item‑egenskapen
            Console.WriteLine("First point coordinates:");
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"X: {firstPoint.X}, Y: {firstPoint.Y}");

            Console.WriteLine("\nAll points in collection:");
            for (int i = 0; i < pathPoints.Count; i++)
            {
                ShapePathPoint point = pathPoints[i];
                Console.WriteLine($"Point {i}: X={point.X}, Y={point.Y}");
            }

            // Skapa en shape path med hjälp av punkterna
            ShapePath path = new ShapePath();

            // Flytta till startpunkten
            path.MoveTo(10, 10);

            foreach (ShapePathPoint point in pathPoints)
            {
                path.LineTo(point.X, point.Y);
            }
            path.Close();

            // Lägg till frihandsform med den konfigurerade pathen
            Shape shape = worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path }
                );

            // Spara resultatet
            workbook.Save("ShapePathPointCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapePathPoint](../../shapepathpoint/)
* class [ShapePathPointCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


