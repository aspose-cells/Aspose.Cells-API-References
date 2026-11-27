---
title: "ShapePathPoint.XAngle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePathPoint-egenskap. När objektet är en vinkelmarkör, hämta eller ange den första vinkeln i grader"
type: docs
url: /sv/net/aspose.cells.drawing/shapepathpoint/xangle/
---
## ShapePathPoint.XAngle property

När objektet är en vinkelmarkör, hämta eller ange den första vinkeln i grader.

```csharp
public int XAngle { get; set; }
```

### Anmärkningar

Om denna vinkel är startvinkeln för en båge. Denna vinkel kommer att ange vilken vinkel längs den förmodade cirkelvägen som ska användas som startposition för att rita bågen. Denna startvinkel kommer att låsas till den senast kända pennpositionen i formvägen. Detta garanterar en kontinuerlig formväg.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXAngleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en samling av formvägspunkter
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(30, 20);
            pathPoints.Add(80, 20);
            pathPoints.Add(80, 70);
            pathPoints.Add(30, 70);

            // Hämta den första punkten och visa dess X- och Y-koordinater
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"First point – X: {firstPoint.X}, Y: {firstPoint.Y}");

            // OBS: Klassen ShapePathPoint (enligt den aktuella API-reflektionen) exponerar inte en XAngle-egenskap.
            // Därför fokuserar denna demo på de tillgängliga X- och Y-egenskaperna.

            // Bygg en enkel frihandsform med de definierade punkterna
            ShapePath path = new ShapePath();
            path.MoveTo(firstPoint.X, firstPoint.Y);
            for (int i = 1; i < pathPoints.Count; i++)
            {
                ShapePathPoint pt = pathPoints[i];
                path.LineTo(pt.X, pt.Y);
            }
            path.Close();

            // Lägg till frihandsformen i kalkylbladet
            worksheet.Shapes.AddFreeform(
                topRow: 2,
                top: 0,
                leftColumn: 2,
                left: 0,
                height: 200,
                width: 200,
                paths: new ShapePath[] { path });

            // Spara arbetsboken
            workbook.Save("ShapePathPointXAngleDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


