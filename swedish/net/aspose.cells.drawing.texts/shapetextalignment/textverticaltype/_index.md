---
title: "ShapeTextAlignment.TextVerticalType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeTextAlignment-egenskap. Hämtar och anger textriktningen"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextalignment/textverticaltype/
---
## ShapeTextAlignment.TextVerticalType property

Hämtar och anger textriktningen.

```csharp
public TextVerticalType TextVerticalType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextVerticalTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textrutaform med korrekta parametrar
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            shape.Text = "Sample Text";

            // Hämta textjusteringen och ställ in vertikal texttyp
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            textAlignment.TextVerticalType = TextVerticalType.Horizontal;

            // Spara arbetsboken
            workbook.Save("TextVerticalTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextVerticalType](../../textverticaltype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


