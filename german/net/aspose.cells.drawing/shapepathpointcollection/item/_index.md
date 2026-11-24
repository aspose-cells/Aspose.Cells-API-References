---
title: "ShapePathPointCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePathPointCollection-Eigenschaft. Gibt den Pfadpunkt der Form nach Index zurück"
type: docs
url: /de/net/aspose.cells.drawing/shapepathpointcollection/item/
---
## ShapePathPointCollection indexer

Liefert den Formpfadpunkt nach Index.

```csharp
public ShapePathPoint this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index |

### Rückgabewert

Gibt ein [`ShapePathPoint`](../../shapepathpoint/) Objekt zurück

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie eine ShapePathPoint-Punktesammlung und fügen Sie Punkte hinzu
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(50, 10);
            pathPoints.Add(50, 50);
            pathPoints.Add(10, 50);

            // Greifen Sie über die Item-Eigenschaft auf Punkte zu
            Console.WriteLine("First point coordinates:");
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"X: {firstPoint.X}, Y: {firstPoint.Y}");

            Console.WriteLine("\nAll points in collection:");
            for (int i = 0; i < pathPoints.Count; i++)
            {
                ShapePathPoint point = pathPoints[i];
                Console.WriteLine($"Point {i}: X={point.X}, Y={point.Y}");
            }

            // Erstellen Sie einen ShapePath mithilfe der Punkte
            ShapePath path = new ShapePath();

            // Zum Ausgangspunkt bewegen
            path.MoveTo(10, 10);

            foreach (ShapePathPoint point in pathPoints)
            {
                path.LineTo(point.X, point.Y);
            }
            path.Close();

            // Fügen Sie eine Freihandform mit dem konfigurierten Pfad hinzu
            Shape shape = worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path }
                );

            // Ergebnis speichern
            workbook.Save("ShapePathPointCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapePathPoint](../../shapepathpoint/)
* class [ShapePathPointCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


