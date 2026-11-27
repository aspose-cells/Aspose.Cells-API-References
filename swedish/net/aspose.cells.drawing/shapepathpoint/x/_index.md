---
title: "ShapePathPoint.X"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePathPoint-egenskap. Hämtar och anger x-koordinat för denna positionskoordinat. Enhet EMUs"
type: docs
url: /sv/net/aspose.cells.drawing/shapepathpoint/x/
---
## ShapePathPoint.X property

Hämtar och anger x-koordinat för denna positionskoordinat. Enhet EMUs.

```csharp
[Obsolete("Use ShapePathPoint.XPixel and ShapePathPoint.XAngle properties instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int X { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället egenskaperna ShapePathPoint.XPixel och ShapePathPoint.XAngle. Denna egenskap kommer att tas bort 12 månader senare från och med augusti 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXDemo
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

            // Spara modifierad arbetsbok
            workbook.Save("ShapePathPointXDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


