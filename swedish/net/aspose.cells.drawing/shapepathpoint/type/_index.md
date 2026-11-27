---
title: "ShapePathPoint.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePathPoint-egenskap. Anger värdetypen för det aktuella objektet"
type: docs
url: /sv/net/aspose.cells.drawing/shapepathpoint/type/
---
## ShapePathPoint.Type property

Anger värdetypen för det aktuella objektet.

```csharp
public ShapePathPointValueType Type { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyTypeDemo
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

                // Lägg till en positionskoordinatpunkt
                int positionPointIndex = pathPoints.Add(100, 50);
                ShapePathPoint positionPoint = pathPoints[positionPointIndex];

                // Visa värdet för Type-egenskapen för positionskoordinaten
                Console.WriteLine($"Position Point Type: {positionPoint.Type}");
                Console.WriteLine($"Position Point Type is Position: {positionPoint.Type == ShapePathPointValueType.Position}");

                // Lägg till en vinkelmarkörpunkt
                int anglePointIndex = pathPoints.Add(0, 0);
                ShapePathPoint anglePoint = pathPoints[anglePointIndex];
                anglePoint.XAngle = 45;
                anglePoint.YAngle = 90;

                // Visa värdet för Type-egenskapen för vinkelmarkören
                Console.WriteLine($"Angle Point Type: {anglePoint.Type}");
                Console.WriteLine($"Angle Point Type is Angle: {anglePoint.Type == ShapePathPointValueType.Angle}");

                // Skapa en formväg och lägg till punkter
                ShapePath path = new ShapePath();
                path.MoveTo(positionPoint.XPixel, positionPoint.YPixel);
                path.ArcTo(anglePoint.XAngle, anglePoint.YAngle, 100, 100);
                path.Close();

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
                workbook.Save("ShapePathPointTypeDemo.xlsx");
                Console.WriteLine("Type property demonstration completed successfully.");
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

* enum [ShapePathPointValueType](../../shapepathpointvaluetype/)
* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


