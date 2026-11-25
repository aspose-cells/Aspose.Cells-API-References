---
title: "Shape.Left"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra nell'unità di pixel"
type: docs
url: /it/net/aspose.cells.drawing/shape/left/
---
## Shape.Left property

Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel.

```csharp
public int Left { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare la proprietà Left
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Imposta la posizione Left iniziale
            shape.Left = 200;
            Console.WriteLine("Shape Left position: " + shape.Left);

            // Modifica la posizione Left in modo condizionale
            if (shape.Left == 200)
            {
                shape.Left = 150;
                Console.WriteLine("Adjusted Shape Left position: " + shape.Left);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


