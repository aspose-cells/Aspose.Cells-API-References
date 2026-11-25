---
title: "Shape.Top"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta lo spostamento verticale della forma dalla sua riga superiore in unità di pixel"
type: docs
url: /it/net/aspose.cells.drawing/shape/top/
---
## Shape.Top property

Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in pixel.

```csharp
public int Top { get; set; }
```

### Osservazioni

Se la forma è nel grafico, rappresenta lo spostamento verticale della forma dal suo bordo superiore.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Imposta la posizione superiore iniziale
            shape.Top = 50;
            Console.WriteLine("Initial Top position: " + shape.Top);

            // Modifica la posizione superiore se è uguale a 3 (dimostrando la logica del caso di test)
            if (shape.Top == 3)
            {
                shape.Top = 1;
            }
            else
            {
                // Per dimostrazione, imposta a 3 e poi applica la logica del caso di test
                shape.Top = 3;
                if (shape.Top == 3)
                {
                    shape.Top = 1;
                    Console.WriteLine("Modified Top position: " + shape.Top);
                }
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


