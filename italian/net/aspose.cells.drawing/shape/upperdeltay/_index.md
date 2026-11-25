---
title: "Shape.UpperDeltaY"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene o imposta lo spostamento verticale della forma dalla sua riga in alto a sinistra"
type: docs
url: /it/net/aspose.cells.drawing/shape/upperdeltay/
---
## Shape.UpperDeltaY property

Ottiene o imposta lo spostamento verticale della forma dalla riga dell'angolo in alto a sinistra.

```csharp
public int UpperDeltaY { get; set; }
```

### Osservazioni

L'intervallo di valore è da 0 a 256.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperDeltaYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare la proprietà UpperDeltaY
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Imposta e visualizza il valore iniziale di UpperDeltaY
            shape.UpperDeltaY = 3;
            Console.WriteLine("Initial UpperDeltaY: " + shape.UpperDeltaY);

            // Modifica il valore di UpperDeltaY
            if (shape.UpperDeltaY == 3)
            {
                shape.UpperDeltaY = 1;
                Console.WriteLine("Modified UpperDeltaY: " + shape.UpperDeltaY);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


