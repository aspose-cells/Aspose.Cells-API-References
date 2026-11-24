---
title: "RenderingFont.RenderingFont"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RenderingFont-Konstruktor. Initialisiert eine neue Instanz von RenderingFont."
type: docs
url: /de/net/aspose.cells.rendering/renderingfont/renderingfont/
---
## RenderingFont constructor

Initialisiert eine neue Instanz von [`RenderingFont`](../)

```csharp
public RenderingFont(string fontName, float fontSize)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontName | String | Schriftname |
| fontSize | Einzeln | Schriftgröße in Punkten. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontMethodCtorWithStringSingleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Eine Schriftart mit dem #ctor(string, single)-Konstruktor erstellen.
            RenderingFont font = new RenderingFont("Arial", 24f);
            font.Bold = true;
            font.Color = System.Drawing.Color.Red;
            
            // Stil erstellen und Schriftart festlegen.
            Style style = workbook.CreateStyle();
            style.Font.Name = font.Name;
            style.Font.Size = (int)font.Size;  // Explicit cast from float to int
            style.Font.IsBold = font.Bold;
            style.Font.Color = font.Color;
            
            // Stil auf Zelle anwenden
            worksheet.Cells["A1"].PutValue("Text with custom font");
            worksheet.Cells["A1"].SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("FontDemoOutput.xlsx");
        }
    }
}
```

### Siehe auch

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


