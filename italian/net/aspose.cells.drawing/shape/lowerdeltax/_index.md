---
title: "Shape.LowerDeltaX"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene o imposta lo spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro"
type: docs
url: /it/net/aspose.cells.drawing/shape/lowerdeltax/
---
## Shape.LowerDeltaX property

Ottiene o imposta lo spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro.

```csharp
public int LowerDeltaX { get; set; }
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
    public class ShapePropertyLowerDeltaXDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Imposta e dimostra la proprietà LowerDeltaX
            shape.LowerDeltaX = 3;
            Console.WriteLine("Initial LowerDeltaX: " + shape.LowerDeltaX);

            // Modifica LowerDeltaX se la condizione è soddisfatta
            if (shape.LowerDeltaX == 3)
            {
                shape.LowerDeltaX = 1;
                Console.WriteLine("Modified LowerDeltaX: " + shape.LowerDeltaX);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


