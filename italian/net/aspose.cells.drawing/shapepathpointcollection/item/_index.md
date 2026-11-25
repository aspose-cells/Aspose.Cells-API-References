---
title: "ShapePathPointCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapePathPointCollection. Ottiene il punto di percorso della forma per indice"
type: docs
url: /it/net/aspose.cells.drawing/shapepathpointcollection/item/
---
## ShapePathPointCollection indexer

Restituisce il punto del percorso della forma per indice.

```csharp
public ShapePathPoint this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice |

### Valore di ritorno

Restituisce l'oggetto [`ShapePathPoint`](../../shapepathpoint/) 

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointCollectionPropertyItemDemo
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

            // Salva il risultato
            workbook.Save("ShapePathPointCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapePathPoint](../../shapepathpoint/)
* class [ShapePathPointCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


