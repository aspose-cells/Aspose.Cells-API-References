---
title: "Shape.IsFilled"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Anger om fyllningsformatet är synligt"
type: docs
url: /sv/net/aspose.cells.drawing/shape/isfilled/
---
## Shape.IsFilled property

Anger om fyllningsformatet är synligt.

```csharp
public bool IsFilled { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Kontrollera och ändra IsFilled-egenskapen
            if (shape.IsFilled == false)
            {
                shape.IsFilled = true;
                shape.FillFormat.ForeColor = System.Drawing.Color.Red;
            }

            // Spara arbetsboken
            workbook.Save("ShapeIsFilledDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


