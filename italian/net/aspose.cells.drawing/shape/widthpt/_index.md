---
title: "Shape.WidthPt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta la larghezza della forma in unità di punto"
type: docs
url: /it/net/aspose.cells.drawing/shape/widthpt/
---
## Shape.WidthPt property

Rappresenta la larghezza della forma, in unità di punti.

```csharp
public double WidthPt { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthPtDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Imposta e ottieni la larghezza in punti
            shape.WidthPt = 150;
            Console.WriteLine("Shape width in points: " + shape.WidthPt);

            // Modifica la larghezza se la condizione è soddisfatta
            if (shape.WidthPt == 150)
            {
                shape.WidthPt = 100;
                Console.WriteLine("Modified shape width in points: " + shape.WidthPt);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


