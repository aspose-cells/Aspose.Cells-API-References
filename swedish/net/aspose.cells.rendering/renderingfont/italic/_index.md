---
title: "RenderingFont.Italic"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RenderingFont-egenskap. Hämtar eller anger kursiv för teckensnittet"
type: docs
url: /sv/net/aspose.cells.rendering/renderingfont/italic/
---
## RenderingFont.Italic property

Hämtar eller sätter kursiv för typsnittet.

```csharp
public bool Italic { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingFontPropertyItalicDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa ett RenderingFont med egenskapen Italic satt
            RenderingFont renderingFont = new RenderingFont("Arial", 16)
            {
                Italic = true,
                Color = Color.Red
            };

            // Applicera teckensnittet på cell A1
            sheet.Cells["A1"].PutValue("Italic Text Example");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";  // Directly use the font name
            style.Font.Size = (int)renderingFont.Size;  // Explicit cast to int
            style.Font.IsItalic = renderingFont.Italic;
            style.Font.Color = renderingFont.Color;
            sheet.Cells["A1"].SetStyle(style);

            // Spara arbetsboken
            workbook.Save("ItalicFontExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


