---
title: "ShapeTextAlignment.IsLockedText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeTextAlignment-egenskapen. Anger om formen är låst när kalkylbladet är skyddat"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextalignment/islockedtext/
---
## ShapeTextAlignment.IsLockedText property

Anger om formen är låst när kalkylbladet är skyddat.

```csharp
public bool IsLockedText { get; set; }
```

### Anmärkningar

Fungerar endast när kalkylbladet är skyddat.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsLockedTextDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            textBox.Text = "Sample Text";

            // Åtkomst till egenskaperna för textjustering
            Aspose.Cells.Drawing.Texts.ShapeTextAlignment textAlignment = textBox.TextBody.TextAlignment;

            // Ställ in och demonstrera egenskapen IsLockedText
            textAlignment.IsLockedText = true;
            Console.WriteLine("Text locked status: " + textAlignment.IsLockedText);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


