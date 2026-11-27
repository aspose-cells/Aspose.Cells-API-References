---
title: "ShapePathPointCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePathPointCollection‑metod. Lägger till en banpunkt i enheten EMU"
type: docs
url: /sv/net/aspose.cells.drawing/shapepathpointcollection/add/
---
## ShapePathPointCollection.Add method

Lägger till en banpunkt i enheten EMU.

```csharp
[Obsolete("Use the MoveTo,LineTo,CubicBezierTo and ArcTo methods in ShapePath instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int x, int y)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| x | Int32 | x‑koordinaten. |
| y | Int32 | y‑koordinaten. |

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället MoveTo,LineTo,CubicBezierTo och ArcTo‑metoderna i ShapePath. Denna metod kommer att tas bort 12 månader senare, från och med augusti 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en shape path point‑samling
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();

            try
            {
                // Anropa Add‑metoden med (Int32, Int32)-parametrar
                pathPoints.Add(50, 10);
                pathPoints.Add(50, 50);
                pathPoints.Add(10, 50);

                // Skapa en formväg och lägg till punkterna
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
                workbook.Save("ShapePathPointCollectionMethodAddWithInt32Int32Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [ShapePathPointCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


