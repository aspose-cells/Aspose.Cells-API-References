---
title: "ShapePathPoint.XPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapePathPoint. Quando l'oggetto è una coordinata di posizione, ottieni o imposta la coordinata x in pixel"
type: docs
url: /it/net/aspose.cells.drawing/shapepathpoint/xpixel/
---
## ShapePathPoint.XPixel property

Quando l'oggetto è una coordinata di posizione, ottieni o imposta la coordinata x in pixel.

```csharp
public int XPixel { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXPixelDemo
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

                // Aggiungi punti con coordinate
                pathPoints.Add(100, 50);
                pathPoints.Add(200, 100);

                // Accedi al primo punto e dimostra la proprietà XPixel
                ShapePathPoint firstPoint = pathPoints[0];

                // Visualizza il valore XPixel (operazione di lettura)
                Console.WriteLine($"Initial XPixel value: {firstPoint.XPixel}");

                // Imposta un nuovo valore per XPixel (poiché è leggibile/scrivibile)
                firstPoint.XPixel = 150;
                Console.WriteLine($"Updated XPixel value: {firstPoint.XPixel}");

                // Crea un percorso di forma e aggiungi i punti
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

                // Aggiungi il secondo punto
                ShapePathPoint secondPoint = pathPoints[1];
                path.LineTo(secondPoint.XPixel, secondPoint.YPixel);
                path.Close();

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
                workbook.Save("XPixelDemo.xlsx");
                Console.WriteLine("XPixel property demonstration completed successfully.");
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


