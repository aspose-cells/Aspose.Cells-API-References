---
title: "ShapePathPoint.XPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePathPoint-Eigenschaft. Wenn das Objekt eine Positionskoordinate ist, die x-Koordinate in Pixel lesen oder festlegen"
type: docs
url: /de/net/aspose.cells.drawing/shapepathpoint/xpixel/
---
## ShapePathPoint.XPixel property

Wenn das Objekt eine Positionskoordinate ist, lese oder schreibe die x‑Koordinate in Pixeln.

```csharp
public int XPixel { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXPixelDemo
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

                // Füge Punkte mit Koordinaten hinzu
                pathPoints.Add(100, 50);
                pathPoints.Add(200, 100);

                // Greife auf den ersten Punkt zu und demonstriere die XPixel-Eigenschaft
                ShapePathPoint firstPoint = pathPoints[0];

                // Zeige den XPixel-Wert (Lesevorgang) an
                Console.WriteLine($"Initial XPixel value: {firstPoint.XPixel}");

                // Setze einen neuen Wert für XPixel (da sie les- und schreibbar ist)
                firstPoint.XPixel = 150;
                Console.WriteLine($"Updated XPixel value: {firstPoint.XPixel}");

                // Erstelle einen Formpfad und füge die Punkte hinzu
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

                // Füge den zweiten Punkt hinzu
                ShapePathPoint secondPoint = pathPoints[1];
                path.LineTo(secondPoint.XPixel, secondPoint.YPixel);
                path.Close();

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
                workbook.Save("XPixelDemo.xlsx");
                Console.WriteLine("XPixel property demonstration completed successfully.");
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


