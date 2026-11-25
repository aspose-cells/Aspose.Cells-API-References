---
title: "Shape.UpperDeltaX"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene o imposta lo spostamento orizzontale della forma dalla colonna dell'angolo superiore sinistro"
type: docs
url: /it/net/aspose.cells.drawing/shape/upperdeltax/
---
## Shape.UpperDeltaX property

Ottiene o imposta lo spostamento orizzontale della forma dalla colonna dell'angolo in alto a sinistra.

```csharp
public int UpperDeltaX { get; set; }
```

### Osservazioni

L'intervallo di valore è da 0 a 1024.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperDeltaXDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Imposta e visualizza la proprietà UpperDeltaX
            shape.UpperDeltaX = 150;
            Console.WriteLine("UpperDeltaX: " + shape.UpperDeltaX);

            // Modifica UpperDeltaX se soddisfa una condizione
            if (shape.UpperDeltaX == 150)
            {
                shape.UpperDeltaX = 100;
                Console.WriteLine("Modified UpperDeltaX: " + shape.UpperDeltaX);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


