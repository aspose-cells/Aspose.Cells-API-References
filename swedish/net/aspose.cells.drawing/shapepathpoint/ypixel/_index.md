---
title: "ShapePathPoint.YPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePathPoint-egenskap. När objektet är en positionskoordinat, hämta eller ange y-koordinaten i pixlar"
type: docs
url: /sv/net/aspose.cells.drawing/shapepathpoint/ypixel/
---
## ShapePathPoint.YPixel property

När objektet är en positionskoordinat, hämta eller ange y‑koordinaten i pixlar.

```csharp
public int YPixel { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa en shape path point‑samling
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // Lägg till en punkt med koordinater
                pathPoints.Add(100, 50);

                // Åtkomst till den första punkten och demonstrera YPixel‑egenskapen
                ShapePathPoint firstPoint = pathPoints[0];

                // Visa det ursprungliga YPixel‑värdet (läsläsning)
                Console.WriteLine($"Initial YPixel value: {firstPoint.YPixel}");

                // Ange ett nytt värde för YPixel (eftersom den är läs/skriv)
                firstPoint.YPixel = 150;
                Console.WriteLine($"Updated YPixel value: {firstPoint.YPixel}");

                // Skapa en shape path och använd punkten
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

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

### Se även

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


