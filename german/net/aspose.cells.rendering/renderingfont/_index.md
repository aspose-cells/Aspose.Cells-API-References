---
title: "Class RenderingFont"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.RenderingFont class. Schriftart für das Rendern"
type: docs
url: /de/net/aspose.cells.rendering/renderingfont/
---
## RenderingFont class

Schriftart für das Rendern.

```csharp
public class RenderingFont
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [RenderingFont](renderingfont/)(string, float) | Initialisiert eine neue Instanz von `RenderingFont` |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Bold](../../aspose.cells.rendering/renderingfont/bold/) { get; set; } | Liest oder setzt Fett für die Schriftart. |
| [Color](../../aspose.cells.rendering/renderingfont/color/) { get; set; } | Liest oder setzt die Farbe für die Schriftart. |
| [Italic](../../aspose.cells.rendering/renderingfont/italic/) { get; set; } | Liest oder setzt Kursiv für die Schriftart. |
| [Name](../../aspose.cells.rendering/renderingfont/name/) { get; } | Liest den Namen der Schriftart. |
| [Size](../../aspose.cells.rendering/renderingfont/size/) { get; } | Liest die Größe der Schriftart in Punkten. |

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontDemo
    {
        public static void RenderingFontExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Hello World!");

            // Erstelle ein RenderingFont-Objekt
            RenderingFont renderingFont = new RenderingFont("Arial", 12)
            {
                Bold = true,
                Italic = true,
                Color = Color.Blue
            };

            // Erstelle ein RenderingWatermark-Objekt mithilfe des RenderingFont
            RenderingWatermark watermark = new RenderingWatermark("Sample Watermark", renderingFont)
            {
                Rotation = 45,
                ScaleToPagePercent = 100,
                Opacity = 0.5f,
                IsBackground = true,
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                OffsetX = 0,
                OffsetY = 0
            };

            // Erstelle PdfSaveOptions und setze das Wasserzeichen
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions
            {
                Watermark = watermark,
                EmbedStandardWindowsFonts = true,
                CalculateFormula = true,
                ExportDocumentStructure = true,
                DisplayDocTitle = true
            };

            // Speichere die Arbeitsmappe als PDF mit dem Wasserzeichen
            workbook.Save("RenderingFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


