---
title: "ShapePathPointCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapePathPointCollection. Aggiunge un punto di percorso in unità EMU"
type: docs
url: /it/net/aspose.cells.drawing/shapepathpointcollection/add/
---
## ShapePathPointCollection.Add method

Aggiunge un punto di percorso in unità EMU.

```csharp
[Obsolete("Use the MoveTo,LineTo,CubicBezierTo and ArcTo methods in ShapePath instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int x, int y)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| x | Int32 | La coordinata x. |
| y | Int32 | La coordinata y. |

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare i metodi MoveTo,LineTo,CubicBezierTo e ArcTo in ShapePath. Questo metodo sarà rimosso 12 mesi dopo, a partire da agosto 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una shape path point collection
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();

            try
            {
                // Chiama il metodo Add con parametri (Int32, Int32)
                pathPoints.Add(50, 10);
                pathPoints.Add(50, 50);
                pathPoints.Add(10, 50);

                // Crea un percorso di forma e aggiungi i punti
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
                workbook.Save("ShapePathPointCollectionMethodAddWithInt32Int32Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ShapePathPointCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


