---
title: "Shape.IsFilled"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Indica se il formato di riempimento è visibile"
type: docs
url: /it/net/aspose.cells.drawing/shape/isfilled/
---
## Shape.IsFilled property

Indica se il formato di riempimento è visibile.

```csharp
public bool IsFilled { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsFilledDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Verifica e modifica la proprietà IsFilled
            if (shape.IsFilled == false)
            {
                shape.IsFilled = true;
                shape.FillFormat.ForeColor = System.Drawing.Color.Red;
            }

            // Salva la cartella di lavoro
            workbook.Save("ShapeIsFilledDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


