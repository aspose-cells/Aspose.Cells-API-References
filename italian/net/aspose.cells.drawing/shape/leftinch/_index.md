---
title: "Shape.LeftInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra in unità di pollici"
type: docs
url: /it/net/aspose.cells.drawing/shape/leftinch/
---
## Shape.LeftInch property

Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pollici.

```csharp
public double LeftInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di esempio con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Imposta e dimostra la proprietà LeftInch
            shape.LeftInch = 3;
            Console.WriteLine("Shape left position (inches): " + shape.LeftInch);

            // Modifica la posizione sinistra se è 3 pollici
            if (shape.LeftInch == 3)
            {
                shape.LeftInch = 1;
                Console.WriteLine("Adjusted shape left position (inches): " + shape.LeftInch);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


