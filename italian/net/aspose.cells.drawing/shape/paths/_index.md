---
title: "Shape.Paths"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene i percorsi di una forma geometrica personalizzata"
type: docs
url: /it/net/aspose.cells.drawing/shape/paths/
---
## Shape.Paths property

Ottiene i percorsi di una forma geometrica personalizzata.

```csharp
public ShapePathCollection Paths { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyPathsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma personalizzata (rettangolo) con parametri corretti
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 1, 1, 100, 150);

            // Verifica se la forma ha percorsi di geometria personalizzata
            if (shape.Paths != null)
            {
                Console.WriteLine("Shape has custom geometry paths:");
                Console.WriteLine($"Number of paths: {shape.Paths.Count}");
                
                // Aggiungi un nuovo percorso alla geometria della forma
                int newPathIndex = shape.Paths.Add();
                Console.WriteLine($"Added new path at index: {newPathIndex}");
            }
            else
            {
                Console.WriteLine("No custom geometry path.");
            }
        }
    }
}
```

### Vedi anche

* class [ShapePathCollection](../../shapepathcollection/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


