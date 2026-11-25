---
title: "Shape.Y"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro in unità di pixel"
type: docs
url: /it/net/aspose.cells.drawing/shape/y/
---
## Shape.Y property

Ottiene e imposta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel.

```csharp
public int Y { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyYDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Imposta e dimostra la proprietà Y
            shape.Y = 200;
            Console.WriteLine("Shape Y position: " + shape.Y);

            // Modifica la posizione Y in base a una condizione
            if (shape.Y == 200)
                shape.Y = 100;

            Console.WriteLine("Updated Shape Y position: " + shape.Y);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


