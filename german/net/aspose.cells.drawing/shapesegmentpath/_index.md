---
title: "Klasse ShapeSegmentPath"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ShapeSegmentPath Klasse. Stellt einen Segmentpfad in einem Pfad der Freiform dar"
type: docs
url: /de/net/aspose.cells.drawing/shapesegmentpath/
---
## ShapeSegmentPath class

Stellt einen Segmentpfad in einem Pfad der Freiform dar.

```csharp
public class ShapeSegmentPath
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Points](../../aspose.cells.drawing/shapesegmentpath/points/) { get; } | Ermittelt die Punkte im Pfadsegment |
| [Type](../../aspose.cells.drawing/shapesegmentpath/type/) { get; } | Ermittelt den Typ des Pfadsegments |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeSegmentPathDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Freiformform zum Arbeitsblatt hinzufügen
            Shape shape = worksheet.Shapes.AddFreeform(0, 0, 0, 0, 200, 200, new ShapePath[] { new ShapePath() });

            // Den Geometriepfad der Form erhalten
            CustomGeometry geometry = shape.Geometry as CustomGeometry;
            ShapePath shapePath = geometry.Paths[0];

            // Greifen Sie auf den ersten Segmentpfad zu (falls vorhanden)
            if (shapePath.PathSegementList.Count > 0)
            {
                ShapeSegmentPath segmentPath = shapePath.PathSegementList[0];

                // Demonstrieren Sie die Eigenschaften von ShapeSegmentPath
                Console.WriteLine("Segment Path Type: " + segmentPath.Type);
                Console.WriteLine("Number of Points: " + segmentPath.Points.Count);

                // Iterieren Sie über die Punkte im Segmentpfad
                foreach (ShapePathPoint point in segmentPath.Points)
                {
                    Console.WriteLine($"Point coordinates: X={point.X}, Y={point.Y}");
                }
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeSegmentPathDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


