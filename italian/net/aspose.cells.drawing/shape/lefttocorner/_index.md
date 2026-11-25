---
title: "Shape.LeftToCorner"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro"
type: docs
url: /it/net/aspose.cells.drawing/shape/lefttocorner/
---
## Shape.LeftToCorner property

Ottiene e imposta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro.

```csharp
public int LeftToCorner { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftToCornerDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con i parametri corretti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Imposta e dimostra la proprietà LeftToCorner
            shape.LeftToCorner = 50;
            Console.WriteLine("Shape LeftToCorner value: " + shape.LeftToCorner);

            // Modifica LeftToCorner se è uguale a un valore specifico
            if (shape.LeftToCorner == 50)
            {
                shape.LeftToCorner = 30;
                Console.WriteLine("Modified LeftToCorner value: " + shape.LeftToCorner);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


