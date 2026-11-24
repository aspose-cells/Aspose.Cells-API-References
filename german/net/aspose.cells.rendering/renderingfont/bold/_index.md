---
title: "RenderingFont.Bold"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RenderingFont property. Gibt zurück oder setzt den Fettdruck der Schriftart"
type: docs
url: /de/net/aspose.cells.rendering/renderingfont/bold/
---
## RenderingFont.Bold property

Liest oder setzt Fett für die Schriftart.

```csharp
public bool Bold { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontPropertyBoldDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Bold Font Example");

            // Erstelle einen Stil für die Zelle
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            worksheet.Cells["A1"].SetStyle(style);

            // PDF-Speicheroptionen mit Wasserzeichen erstellen, das fette Schrift demonstriert
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Rendering-Schriftart mit Fettdruck-Eigenschaft erstellen
            RenderingFont font = new RenderingFont("Arial", 36)
            {
                Bold = true,
                Color = System.Drawing.Color.Red
            };
            
            // Wasserzeichen mit fetter Schriftart erstellen
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Opacity = 0.3f
            };
            pdfSaveOptions.Watermark = watermark;

            // Speichere die Arbeitsmappe
            workbook.Save("BoldFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### Siehe auch

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


