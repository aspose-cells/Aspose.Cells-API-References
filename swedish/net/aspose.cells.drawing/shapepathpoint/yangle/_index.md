---
title: "ShapePathPoint.YAngle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePathPoint-egenskap. När objektet är en vinkelmarkör, hämta eller ange den andra vinkeln i grader"
type: docs
url: /sv/net/aspose.cells.drawing/shapepathpoint/yangle/
---
## ShapePathPoint.YAngle property

När objektet är en vinkelmarkör, hämta eller ange den andra vinkeln i grader.

```csharp
public int YAngle { get; set; }
```

### Anmärkningar

Om denna vinkel är svängvinkeln för en båge. Denna vinkel anger hur långt, i vinkelmässig mening, längs den påstådda cirkelbanan bågen kommer att förlängas. Förlängningen från startvinkeln kommer alltid att vara i medurs riktning runt den påstådda cirkeln.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYAngleDemo
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

                // Lägg till punkter med vinkelmarkörer (med XAngle och YAngle)
                ShapePathPoint point1 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point1.XAngle = 45;  // First angle in degrees
                point1.YAngle = 90;  // Second angle in degrees

                // Visa YAngle‑värdet
                Console.WriteLine($"Point 1 YAngle: {point1.YAngle} degrees");

                // Skapa en annan punkt med olika vinklar
                ShapePathPoint point2 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point2.XAngle = 30;
                point2.YAngle = 60;

                // Visa YAngle‑värdet
                Console.WriteLine($"Point 2 YAngle: {point2.YAngle} degrees");

                // Skapa en formväg och lägg till en båge med hjälp av vinkelmarkörer
                ShapePath path = new ShapePath();
                path.ArcTo(point1.XAngle, point1.YAngle, 100, 100);

                // Lägg till frihandsform i kalkylbladet
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Spara arbetsboken
                workbook.Save("YAngleDemo.xlsx");
                Console.WriteLine("YAngle property demonstration completed successfully.");
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


