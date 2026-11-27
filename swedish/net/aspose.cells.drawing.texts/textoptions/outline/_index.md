---
title: "TextOptions.Outline"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextOptions egenskap. Representerar konturformatet för texten"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textoptions/outline/
---
## TextOptions.Outline property

Representerar konturformatet för texten.

```csharp
public LineFormat Outline { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyOutlineDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form med text
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
            shape.Text = "Sample Text";

            // Åtkomst till textalternativ
            TextOptions textOptions = shape.TextOptions;

            // Konfigurera konturegenskaper
            LineFormat outline = textOptions.Outline;
            outline.Weight = 2.48; // Set outline weight
            outline.DashStyle = MsoLineDashStyle.Solid; // Set line style
            outline.CompoundType = MsoLineStyle.Single; // Set compound type

            // Spara arbetsboken
            workbook.Save("TextOutlineDemo.xlsx");
        }
    }
}
```

### Se även

* class [LineFormat](../../../aspose.cells.drawing/lineformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


