---
title: "Shape.HeightInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta l'altezza della forma in unità di pollici"
type: docs
url: /it/net/aspose.cells.drawing/shape/heightinch/
---
## Shape.HeightInch property

Rappresenta l'altezza della forma, in unità di pollici.

```csharp
public double HeightInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Imposta e ottieni l'altezza in pollici
            shape.HeightInch = 3;
            Console.WriteLine("Shape height (inches): " + shape.HeightInch);

            // Modifica l'altezza se la condizione è soddisfatta
            if (shape.HeightInch == 3)
            {
                shape.HeightInch = 1;
                Console.WriteLine("Modified shape height (inches): " + shape.HeightInch);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


