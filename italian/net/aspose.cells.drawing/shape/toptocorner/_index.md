---
title: "Shape.TopToCorner"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro in unità di pixel"
type: docs
url: /it/net/aspose.cells.drawing/shape/toptocorner/
---
## Shape.TopToCorner property

Ottiene e imposta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in pixel.

```csharp
public int TopToCorner { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopToCornerDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Imposta e visualizza la proprietà TopToCorner
            shape.TopToCorner = 50;
            Console.WriteLine("Shape TopToCorner: " + shape.TopToCorner);

            // Modifica la proprietà TopToCorner
            if (shape.TopToCorner == 50)
            {
                shape.TopToCorner = 20;
                Console.WriteLine("Updated Shape TopToCorner: " + shape.TopToCorner);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


