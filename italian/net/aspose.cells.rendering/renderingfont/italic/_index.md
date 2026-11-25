---
title: "RenderingFont.Italic"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RenderingFont. Ottiene o imposta il corsivo per il carattere"
type: docs
url: /it/net/aspose.cells.rendering/renderingfont/italic/
---
## RenderingFont.Italic property

Ottiene o imposta il corsivo per il font.

```csharp
public bool Italic { get; set; }
```

### Esempi

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

            // Crea un RenderingFont con la proprietà Italic impostata
            RenderingFont renderingFont = new RenderingFont("Arial", 16)
            {
                Italic = true,
                Color = Color.Red
            };

            // Applica il carattere alla cella A1
            sheet.Cells["A1"].PutValue("Italic Text Example");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";  // Directly use the font name
            style.Font.Size = (int)renderingFont.Size;  // Explicit cast to int
            style.Font.IsItalic = renderingFont.Italic;
            style.Font.Color = renderingFont.Color;
            sheet.Cells["A1"].SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("ItalicFontExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


