---
title: "Shape.ActualLowerRightRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottieni la riga inferiore reale"
type: docs
url: /it/net/aspose.cells.drawing/shape/actuallowerrightrow/
---
## Shape.ActualLowerRightRow property

Ottieni la riga inferiore effettiva.

```csharp
public int ActualLowerRightRow { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyActualLowerRightRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di esempio (rettangolo)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 100);

            // Ottieni la riga inferiore destra reale della forma
            int actualLowerRightRow = shape.ActualLowerRightRow;

            // Restituisci il risultato
            Console.WriteLine("Actual Lower Right Row of the shape: " + actualLowerRightRow);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


