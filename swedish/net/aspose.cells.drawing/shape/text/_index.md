---
title: "Shape.Text"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape egenskap. Hämtar och sätter texten för denna form"
type: docs
url: /sv/net/aspose.cells.drawing/shape/text/
---
## Shape.Text property

Hämtar och anger texten för den här formen.

```csharp
public string Text { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform med korrekta parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Sätt text om null
            if (shape.Text == null)
            {
                shape.Text = "This is a test.";
            }

            // Ändra texten
            shape.Text = "Updated text demo";

            // Spara arbetsboken
            workbook.Save("ShapeTextDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


