---
title: "Shape.X"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro in unità di pixel"
type: docs
url: /it/net/aspose.cells.drawing/shape/x/
---
## Shape.X property

Ottiene e imposta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro, in unità di pixel.

```csharp
public int X { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyXDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Imposta la posizione X iniziale
            shape.X = 200;
            Console.WriteLine("Initial X position: " + shape.X);

            // Modifica la posizione X se è uguale a 3 (dimostrando la logica del caso di test)
            if (shape.X == 3)
            {
                shape.X = 1;
            }
            else
            {
                // Per dimostrazione, cambia la posizione X a 300
                shape.X = 300;
            }

            Console.WriteLine("Final X position: " + shape.X);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


