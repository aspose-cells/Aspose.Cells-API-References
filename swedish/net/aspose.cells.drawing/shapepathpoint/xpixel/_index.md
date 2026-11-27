---
title: "ShapePathPoint.XPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePathPoint-egenskap. När objektet är en positionskoordinat, hämta eller ange x-koordinaten i pixlar"
type: docs
url: /sv/net/aspose.cells.drawing/shapepathpoint/xpixel/
---
## ShapePathPoint.XPixel property

När objektet är en positionskoordinat, hämta eller ange x‑koordinaten i pixlar.

```csharp
public int XPixel { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa en shape path point‑samling
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // Lägg till punkter med koordinater
                pathPoints.Add(100, 50);
                pathPoints.Add(200, 100);

                // Åtkomst till den första punkten och demonstrera XPixel-egenskapen
                ShapePathPoint firstPoint = pathPoints[0];

                // Visa XPixel-värdet (läsoperation)
                Console.WriteLine($"Initial XPixel value: {firstPoint.XPixel}");

                // Ange ett nytt värde för XPixel (eftersom den är läs/skriv)
                firstPoint.XPixel = 150;
                Console.WriteLine($"Updated XPixel value: {firstPoint.XPixel}");

                // Skapa en formväg och lägg till punkterna
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

                // Lägg till den andra punkten
                ShapePathPoint secondPoint = pathPoints[1];
                path.LineTo(secondPoint.XPixel, secondPoint.YPixel);
                path.Close();

                // Lägg till en frihandsform i arbetsbladet
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Spara arbetsboken
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

### Se även

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


