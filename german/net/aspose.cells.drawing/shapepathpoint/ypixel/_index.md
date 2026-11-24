---
title: "ShapePathPoint.YPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePathPoint-Eigenschaft. Wenn das Objekt eine Positionskoordinate ist, erhalten oder setzen Sie die y-Koordinate in Pixeln"
type: docs
url: /de/net/aspose.cells.drawing/shapepathpoint/ypixel/
---
## ShapePathPoint.YPixel property

Wenn das Objekt eine Positionskoordinate ist, lese oder schreibe die y‑Koordinate in Pixeln.

```csharp
public int YPixel { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYPixelDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstellen Sie eine ShapePathPoint-Punktesammlung
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // Fügen Sie einen Punkt mit Koordinaten hinzu
                pathPoints.Add(100, 50);

                // Greifen Sie auf den ersten Punkt zu und demonstrieren Sie die YPixel-Eigenschaft
                ShapePathPoint firstPoint = pathPoints[0];

                // Zeigen Sie den initialen YPixel-Wert an (Lesevorgang)
                Console.WriteLine($"Initial YPixel value: {firstPoint.YPixel}");

                // Setzen Sie einen neuen Wert für YPixel (da es les- und schreibbar ist)
                firstPoint.YPixel = 150;
                Console.WriteLine($"Updated YPixel value: {firstPoint.YPixel}");

                // Erstellen Sie einen ShapePath und verwenden Sie den Punkt
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

                // Eine Freiformform zum Arbeitsblatt hinzufügen
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Speichere die Arbeitsmappe
                workbook.Save("YPixelDemo.xlsx");
                Console.WriteLine("YPixel property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


