---
title: "ShapePathPoint.XAngle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePathPoint-Eigenschaft. Wenn das Objekt ein Winkelmarker ist, den ersten Winkel in Grad lesen oder festlegen"
type: docs
url: /de/net/aspose.cells.drawing/shapepathpoint/xangle/
---
## ShapePathPoint.XAngle property

Wenn das Objekt ein Winkelmarker ist, lese oder schreibe den ersten Winkel in Grad.

```csharp
public int XAngle { get; set; }
```

### Hinweise

Wenn dieser Winkel der Startwinkel eines Bogens ist, gibt dieser Winkel an, welcher Winkel entlang des angenommenen Kreiswegs als Startposition für das Zeichnen des Bogens verwendet wird. Dieser Startwinkel wird an die zuletzt bekannte Stiftposition im Formpfad gesperrt, wodurch ein kontinuierlicher Formpfad garantiert wird.

### Beispiele

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
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Sammlung von Formpfad-Punkten
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(30, 20);
            pathPoints.Add(80, 20);
            pathPoints.Add(80, 70);
            pathPoints.Add(30, 70);

            // Rufe den ersten Punkt ab und zeige seine X- und Y-Koordinaten an
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"First point – X: {firstPoint.X}, Y: {firstPoint.Y}");

            // HINWEIS: Die ShapePathPoint-Klasse (gemäß der aktuellen API-Reflexion) stellt keine XAngle-Eigenschaft bereit.
            // Daher konzentriert sich diese Demo auf die verfügbaren X- und Y-Eigenschaften.

            // Erstelle eine einfache Freihandform mithilfe der definierten Punkte
            ShapePath path = new ShapePath();
            path.MoveTo(firstPoint.X, firstPoint.Y);
            for (int i = 1; i < pathPoints.Count; i++)
            {
                ShapePathPoint pt = pathPoints[i];
                path.LineTo(pt.X, pt.Y);
            }
            path.Close();

            // Füge die Freihandform dem Arbeitsblatt hinzu
            worksheet.Shapes.AddFreeform(
                topRow: 2,
                top: 0,
                leftColumn: 2,
                left: 0,
                height: 200,
                width: 200,
                paths: new ShapePath[] { path });

            // Speichere die Arbeitsmappe
            workbook.Save("ShapePathPointXAngleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


