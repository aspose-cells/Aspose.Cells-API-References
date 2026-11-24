---
title: "ShapePathPoint.YAngle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePathPoint-Eigenschaft. Wenn das Objekt ein Winkelmarker ist, erhalten oder setzen Sie den zweiten Winkel in Grad"
type: docs
url: /de/net/aspose.cells.drawing/shapepathpoint/yangle/
---
## ShapePathPoint.YAngle property

Wenn das Objekt ein Winkelmarker ist, lese oder schreibe den zweiten Winkel in Grad.

```csharp
public int YAngle { get; set; }
```

### Hinweise

Falls dieser Winkel der Schwenkwinkel eines Bogens ist. Dieser Winkel gibt an, wie weit entlang des angenommenen Kreiswegs der Bogen winkelweise erweitert wird. Die Erweiterung vom Startwinkel aus erfolgt stets im Uhrzeigersinn um den angenommenen Kreis.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstellen Sie eine ShapePathPoint-Punktesammlung
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // Fügen Sie Punkte mit Winkelmarkern hinzu (unter Verwendung von XAngle und YAngle)
                ShapePathPoint point1 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point1.XAngle = 45;  // First angle in degrees
                point1.YAngle = 90;  // Second angle in degrees

                // Zeigen Sie den YAngle-Wert an
                Console.WriteLine($"Point 1 YAngle: {point1.YAngle} degrees");

                // Erstelle einen weiteren Punkt mit unterschiedlichen Winkeln
                ShapePathPoint point2 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point2.XAngle = 30;
                point2.YAngle = 60;

                // Zeigen Sie den YAngle-Wert an
                Console.WriteLine($"Point 2 YAngle: {point2.YAngle} degrees");

                // Erstelle einen Formpfad und füge einen Bogen mit Winkelmarkern hinzu
                ShapePath path = new ShapePath();
                path.ArcTo(point1.XAngle, point1.YAngle, 100, 100);

                // Freiformform zum Arbeitsblatt hinzufügen
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


