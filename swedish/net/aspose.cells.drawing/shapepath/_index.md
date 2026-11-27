---
title: "Klass ShapePath"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ShapePath-klass. Representerar en skapningssökväg bestående av en serie rörelser, linjer och kurvor som när de kombineras bildar en geometrisk form"
type: docs
url: /sv/net/aspose.cells.drawing/shapepath/
---
## ShapePath class

Representerar en skapandeväg bestående av en serie rörelser, linjer och kurvor som när de kombineras bildar en geometrisk form.

```csharp
public class ShapePath
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ShapePath](shapepath/)() | Initierar en ny instans av `ShapePath`-klassen. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [HeightPixel](../../aspose.cells.drawing/shapepath/heightpixel/) { get; set; } | Hämtar höjden på denna bana i enhet pixlar. |
| [PathSegementList](../../aspose.cells.drawing/shapepath/pathsegementlist/) { get; } | (**Obsolete.**) Hämtar [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) listan |
| [PathSegments](../../aspose.cells.drawing/shapepath/pathsegments/) { get; } | Hämtar [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) listan |
| [WidthPixel](../../aspose.cells.drawing/shapepath/widthpixel/) { get; set; } | Hämtar bredden på denna bana i enhet pixlar. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ArcTo](../../aspose.cells.drawing/shapepath/arcto/)(float, float, float, float) | Lägger till en elliptisk båge till den aktuella figuren. Startpunkten är slutpunkten för den aktuella figuren. |
| [Close](../../aspose.cells.drawing/shapepath/close/)() | Stänger den aktuella figuren och startar en ny figur. Om den aktuella figuren innehåller en sekvens av sammanhängande linjer och kurvor, stänger metoden loopen genom att ansluta en linje från slutpunkten till startpunkten. |
| [CubicBezierTo](../../aspose.cells.drawing/shapepath/cubicbezierto/)(float, float, float, float, float, float) | Lägger till en kubisk Bézier-kurva till den aktuella figuren. Startpunkten är slutpunkten för den aktuella figuren.Enhet: Pixel. |
| [LineTo](../../aspose.cells.drawing/shapepath/lineto/)(float, float) | Lägger till ett linjesegment till den aktuella figuren. Startpunkten är slutpunkten för den aktuella figuren.Enhet: Pixel. |
| [MoveTo](../../aspose.cells.drawing/shapepath/moveto/)(float, float) | Startar en ny figur från den angivna punkten utan att stänga den aktuella figuren. Alla efterföljande punkter som läggs till i banan läggs till i denna nya figur.Enhet: Pixel. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapePathDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en anpassad form med alla nödvändiga parametrar
            Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 100, 0, 0);
            
            // Åtkomst till ShapePathCollection
            ShapePathCollection shapePaths = customShape.Paths;

            // Lägg till en ny bana och få åtkomst till den
            int pathIndex = shapePaths.Add();
            ShapePath newPath = shapePaths[pathIndex];

            // Skriv ut antalet banor
            Console.WriteLine("Number of paths in the ShapePathCollection: " + shapePaths.Count.ToString());

            // Spara arbetsboken
            workbook.Save("ShapePathDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


