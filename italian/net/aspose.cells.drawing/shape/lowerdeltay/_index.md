---
title: "Shape.LowerDeltaY"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene o imposta lo spostamento verticale della forma dalla sua riga dell'angolo inferiore destro"
type: docs
url: /it/net/aspose.cells.drawing/shape/lowerdeltay/
---
## Shape.LowerDeltaY property

Ottiene o imposta lo spostamento verticale della forma dalla riga dell'angolo inferiore destro.

```csharp
public int LowerDeltaY { get; set; }
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
    public class ShapePropertyLowerDeltaYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di esempio con i parametri corretti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Imposta e dimostra la proprietà LowerDeltaY
            shape.LowerDeltaY = 20;
            Console.WriteLine("Initial LowerDeltaY: " + shape.LowerDeltaY);

            // Modifica LowerDeltaY in modo condizionale
            if (shape.LowerDeltaY == 20)
            {
                shape.LowerDeltaY = 10;
                Console.WriteLine("Modified LowerDeltaY: " + shape.LowerDeltaY);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


