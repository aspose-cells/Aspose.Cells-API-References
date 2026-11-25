---
title: "Shape.TopInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta lo spostamento verticale della forma dalla sua riga superiore in unità di pollici"
type: docs
url: /it/net/aspose.cells.drawing/shape/topinch/
---
## Shape.TopInch property

Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in pollici.

```csharp
public double TopInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopInchDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Imposta e dimostra la proprietà TopInch
            shape.TopInch = 3;
            Console.WriteLine("Shape Top position (inches): " + shape.TopInch);

            // Modifica TopInch se è uguale a 3
            if (shape.TopInch == 3)
            {
                shape.TopInch = 1;
                Console.WriteLine("Modified Shape Top position (inches): " + shape.TopInch);
            }

            // Salva la cartella di lavoro
            workbook.Save("ShapeTopInchDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


