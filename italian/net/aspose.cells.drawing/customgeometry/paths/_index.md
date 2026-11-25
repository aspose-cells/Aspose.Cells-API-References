---
title: "CustomGeometry.Paths"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CustomGeometry. Ottiene le informazioni sulla raccolta di percorsi quando la forma è un autoshape NotPrimitive"
type: docs
url: /it/net/aspose.cells.drawing/customgeometry/paths/
---
## CustomGeometry.Paths property

Ottiene le informazioni della raccolta percorsi quando la forma è un autoshape NotPrimitive

```csharp
public ShapePathCollection Paths { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CustomGeometryPropertyPathsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma personalizzata con geometria non primitiva (parametri fissi)
            var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 10, 10, 400, 400);
            
            // Accedi alla geometria personalizzata tramite cast esplicito
            CustomGeometry geometry = (CustomGeometry)shape.Geometry;
            
            // Ottieni la raccolta di percorsi
            ShapePathCollection paths = geometry.Paths;
            Console.WriteLine($"Initial path count: {paths.Count}");

            // Crea un nuovo percorso di forma usando i comandi di disegno
            paths.Add(); // Creates a new path in the collection
            ShapePath newPath = paths[paths.Count - 1];
            newPath.MoveTo(0, 0);
            newPath.LineTo(10000, 0);
            newPath.LineTo(10000, 10000);
            newPath.LineTo(0, 10000);
            newPath.Close();

            // Nessun Add esplicito necessario poiché il percorso è stato creato nella raccolta
            Console.WriteLine($"New path count after modification: {paths.Count}");

            // Salva per dimostrare le modifiche persistenti
            workbook.Save("CustomGeometryPathsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapePathCollection](../../shapepathcollection/)
* class [CustomGeometry](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


