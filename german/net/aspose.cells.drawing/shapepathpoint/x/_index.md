---
title: "ShapePathPoint.X"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePathPoint-Eigenschaft. Gibt die x-Koordinate für diese Positionskoordinate zurück und setzt sie. Einheit EMUs"
type: docs
url: /de/net/aspose.cells.drawing/shapepathpoint/x/
---
## ShapePathPoint.X property

Gibt die x-Koordinate für diese Positionskoordinate zurück und setzt sie. Einheit EMUs.

```csharp
[Obsolete("Use ShapePathPoint.XPixel and ShapePathPoint.XAngle properties instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int X { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaften ShapePathPoint.XPixel und ShapePathPoint.XAngle. Diese Eigenschaft wird 12 Monate später, seit August 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie eine ShapePathPoint-Punktesammlung und fügen Sie Punkte hinzu
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(50, 10);
            pathPoints.Add(50, 50);
            pathPoints.Add(10, 50);

            // Greifen Sie über die Item-Eigenschaft auf Punkte zu
            Console.WriteLine("First point coordinates:");
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"X: {firstPoint.X}, Y: {firstPoint.Y}");

            Console.WriteLine("\nAll points in collection:");
            for (int i = 0; i < pathPoints.Count; i++)
            {
                ShapePathPoint point = pathPoints[i];
                Console.WriteLine($"Point {i}: X={point.X}, Y={point.Y}");
            }

            // Erstellen Sie einen ShapePath mithilfe der Punkte
            ShapePath path = new ShapePath();

            // Zum Ausgangspunkt bewegen
            path.MoveTo(10, 10);

            foreach (ShapePathPoint point in pathPoints)
            {
                path.LineTo(point.X, point.Y);
            }
            path.Close();

            // Fügen Sie eine Freihandform mit dem konfigurierten Pfad hinzu
            Shape shape = worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path }
                );

            // Modifizierte Arbeitsmappe speichern
            workbook.Save("ShapePathPointXDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


