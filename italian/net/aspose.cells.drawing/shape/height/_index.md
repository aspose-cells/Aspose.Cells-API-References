---
title: "Shape.Height"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta l'altezza della forma in unità di pixel"
type: docs
url: /it/net/aspose.cells.drawing/shape/height/
---
## Shape.Height property

Rappresenta l'altezza della shape, in unità di pixel.

```csharp
public int Height { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Imposta l'altezza iniziale
            shape.Height = 150;
            Console.WriteLine("Initial height: " + shape.Height);

            // Modifica l'altezza in modo condizionale
            if (shape.Height == 150)
            {
                shape.Height = 100;
                Console.WriteLine("Modified height: " + shape.Height);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


