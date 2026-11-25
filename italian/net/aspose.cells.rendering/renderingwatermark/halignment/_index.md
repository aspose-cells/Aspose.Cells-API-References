---
title: "RenderingWatermark.HAlignment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RenderingWatermark. Ottiene o imposta l'allineamento orizzontale della filigrana alla pagina"
type: docs
url: /it/net/aspose.cells.rendering/renderingwatermark/halignment/
---
## RenderingWatermark.HAlignment property

Ottiene o imposta l'allineamento orizzontale della filigrana rispetto alla pagina.

```csharp
public TextAlignmentType HAlignment { get; set; }
```

### Osservazioni

Solo Left, Center, Right sono validi. Il valore predefinito è Left.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyHAlignmentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Watermark HAlignment Demo");

            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Crea e configura filigrana con impostazioni HAlignment diverse
            RenderingFont font = new RenderingFont("Arial", 48)
            {
                Bold = true,
                Color = System.Drawing.Color.Blue
            };

            // Crea filigrana con allineamento Center
            RenderingWatermark watermark = new RenderingWatermark("CENTER ALIGNED", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Opacity = 0.5f
            };
            pdfSaveOptions.Watermark = watermark;

            // Salva con filigrana allineata al centro
            workbook.Save("WatermarkCenterAlignment.pdf", pdfSaveOptions);

            // Cambia allineamento a Left
            watermark.HAlignment = TextAlignmentType.Left;
            workbook.Save("WatermarkLeftAlignment.pdf", pdfSaveOptions);

            // Cambia allineamento a Right
            watermark.HAlignment = TextAlignmentType.Right;
            workbook.Save("WatermarkRightAlignment.pdf", pdfSaveOptions);
        }
    }
}
```

### Vedi anche

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


