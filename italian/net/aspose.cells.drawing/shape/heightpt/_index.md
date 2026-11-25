---
title: "Shape.HeightPt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta l'altezza della forma in unità di punti"
type: docs
url: /it/net/aspose.cells.drawing/shape/heightpt/
---
## Shape.HeightPt property

Rappresenta l'altezza della forma, in unità di punti.

```csharp
public double HeightPt { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di esempio con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 100);

            // Imposta e ottieni la proprietà HeightPt
            shape.HeightPt = 50;
            Console.WriteLine("Shape height in points: " + shape.HeightPt);

            // Modifica l'altezza se soddisfa una condizione
            if (shape.HeightPt == 50)
            {
                shape.HeightPt = 30;
                Console.WriteLine("Modified shape height: " + shape.HeightPt);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


