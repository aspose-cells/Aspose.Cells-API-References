---
title: "ShapePathPoint.YPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapePathPoint. Quando l'oggetto è una coordinata di posizione, ottieni o imposta la coordinata y in pixel"
type: docs
url: /it/net/aspose.cells.drawing/shapepathpoint/ypixel/
---
## ShapePathPoint.YPixel property

Quando l'oggetto è una coordinata di posizione, ottieni o imposta la coordinata y in pixel.

```csharp
public int YPixel { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYPixelDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea una shape path point collection
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // Aggiungi un punto con coordinate
                pathPoints.Add(100, 50);

                // Accedi al primo punto e dimostra la proprietà YPixel
                ShapePathPoint firstPoint = pathPoints[0];

                // Visualizza il valore iniziale di YPixel (operazione di lettura)
                Console.WriteLine($"Initial YPixel value: {firstPoint.YPixel}");

                // Imposta un nuovo valore per YPixel (poiché è leggibile/scrivibile)
                firstPoint.YPixel = 150;
                Console.WriteLine($"Updated YPixel value: {firstPoint.YPixel}");

                // Crea un shape path e utilizza il punto
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

                // Aggiungi una forma libera al foglio di lavoro
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Salva la cartella di lavoro
                workbook.Save("YPixelDemo.xlsx");
                Console.WriteLine("YPixel property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


