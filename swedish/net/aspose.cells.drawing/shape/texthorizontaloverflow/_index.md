---
title: "Shape.TextHorizontalOverflow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar och sätter den horisontella översvämningstypen för texten i formen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/texthorizontaloverflow/
---
## Shape.TextHorizontalOverflow property

Hämtar och anger den horisontella översvämningstypen för texten i formen som innehåller text.

```csharp
public TextOverflowType TextHorizontalOverflow { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextHorizontalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textrutaform med korrekta parametrar
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            textBox.Text = "This is a long text that will demonstrate text horizontal overflow functionality";

            // Ställ in initial översvämningstyp till Clip
            textBox.TextHorizontalOverflow = TextOverflowType.Clip;
            Console.WriteLine("TextHorizontalOverflow set to Clip (text will be clipped)");

            // Ändra översvämningstyp till Overflow
            textBox.TextHorizontalOverflow = TextOverflowType.Overflow;
            Console.WriteLine("TextHorizontalOverflow changed to Overflow (text will overflow)");

            // Spara arbetsboken
            workbook.Save("TextHorizontalOverflowDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextOverflowType](../../textoverflowtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


