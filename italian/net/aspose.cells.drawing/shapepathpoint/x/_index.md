---
title: "ShapePathPoint.X"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapePathPoint. Ottiene e imposta la coordinata x per questa coordinata di posizione. Unit EMUs"
type: docs
url: /it/net/aspose.cells.drawing/shapepathpoint/x/
---
## ShapePathPoint.X property

Ottiene e imposta la coordinata x per questa coordinata di posizione. Unit EMUs.

```csharp
[Obsolete("Use ShapePathPoint.XPixel and ShapePathPoint.XAngle properties instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int X { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare le proprietà ShapePathPoint.XPixel e ShapePathPoint.XAngle. Questa proprietà sarà rimossa 12 mesi dopo, a partire da agosto 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una shape path point collection e aggiungi i punti
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(50, 10);
            pathPoints.Add(50, 50);
            pathPoints.Add(10, 50);

            // Accedi ai punti usando la proprietà Item
            Console.WriteLine("First point coordinates:");
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"X: {firstPoint.X}, Y: {firstPoint.Y}");

            Console.WriteLine("\nAll points in collection:");
            for (int i = 0; i < pathPoints.Count; i++)
            {
                ShapePathPoint point = pathPoints[i];
                Console.WriteLine($"Point {i}: X={point.X}, Y={point.Y}");
            }

            // Crea un shape path usando i punti
            ShapePath path = new ShapePath();

            // Sposta al punto di partenza
            path.MoveTo(10, 10);

            foreach (ShapePathPoint point in pathPoints)
            {
                path.LineTo(point.X, point.Y);
            }
            path.Close();

            // Aggiungi una forma libera con il percorso configurato
            Shape shape = worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path }
                );

            // Salvare la cartella di lavoro modificata
            workbook.Save("ShapePathPointXDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


