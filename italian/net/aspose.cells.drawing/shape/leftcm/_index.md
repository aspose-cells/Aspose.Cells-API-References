---
title: "Shape.LeftCM"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra in unità di centimetri"
type: docs
url: /it/net/aspose.cells.drawing/shape/leftcm/
---
## Shape.LeftCM property

Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di centimetri.

```csharp
public double LeftCM { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftCMDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Imposta e ottieni la proprietà LeftCM
            shape.LeftCM = 3.0;
            Console.WriteLine("Shape left position (cm): " + shape.LeftCM);

            // Modifica la posizione sinistra se è 3 cm
            if (shape.LeftCM == 3.0)
            {
                shape.LeftCM = 1.0;
                Console.WriteLine("Adjusted shape left position (cm): " + shape.LeftCM);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


