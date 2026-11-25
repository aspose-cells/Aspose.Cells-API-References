---
title: "RenderingFont.Bold"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RenderingFont. Ottiene o imposta il grassetto per il carattere"
type: docs
url: /it/net/aspose.cells.rendering/renderingfont/bold/
---
## RenderingFont.Bold property

Ottiene o imposta il grassetto per il font.

```csharp
public bool Bold { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Bold Font Example");

            // Crea uno stile per la cella
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Crea opzioni di salvataggio PDF con filigrana che dimostra il carattere grassetto
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Crea carattere di rendering con proprietà grassetto
            RenderingFont font = new RenderingFont("Arial", 36)
            {
                Bold = true,
                Color = System.Drawing.Color.Red
            };
            
            // Crea filigrana con carattere grassetto
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Opacity = 0.3f
            };
            pdfSaveOptions.Watermark = watermark;

            // Salva la cartella di lavoro
            workbook.Save("BoldFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### Vedi anche

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


