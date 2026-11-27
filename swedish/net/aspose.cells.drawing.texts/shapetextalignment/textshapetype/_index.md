---
title: "ShapeTextAlignment.TextShapeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeTextAlignment‑egenskap. Hämtar och anger transformtypen för text"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextalignment/textshapetype/
---
## ShapeTextAlignment.TextShapeType property

Hämtar och anger transformeringstypen för text.

```csharp
public AutoShapeType TextShapeType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextShapeTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);

            // Hämta textjusteringen för formen
            ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;

            // Ställ in egenskapen TextShapeType
            shapeTextAlignment.TextShapeType = AutoShapeType.TextBox;

            // Spara arbetsboken
            workbook.Save("TextShapeTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [AutoShapeType](../../../aspose.cells.drawing/autoshapetype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


