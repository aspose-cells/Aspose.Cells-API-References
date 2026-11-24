---
title: "RenderingFont.Italic"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RenderingFont-Eigenschaft. Gibt die Kursivstellung der Schriftart zurück oder legt sie fest."
type: docs
url: /de/net/aspose.cells.rendering/renderingfont/italic/
---
## RenderingFont.Italic property

Liest oder setzt Kursiv für die Schriftart.

```csharp
public bool Italic { get; set; }
```

### Beispiele

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

            // Ein RenderingFont mit gesetzter Italic‑Eigenschaft erstellen.
            RenderingFont renderingFont = new RenderingFont("Arial", 16)
            {
                Italic = true,
                Color = Color.Red
            };

            // Die Schriftart auf Zelle A1 anwenden.
            sheet.Cells["A1"].PutValue("Italic Text Example");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";  // Directly use the font name
            style.Font.Size = (int)renderingFont.Size;  // Explicit cast to int
            style.Font.IsItalic = renderingFont.Italic;
            style.Font.Color = renderingFont.Color;
            sheet.Cells["A1"].SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("ItalicFontExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


