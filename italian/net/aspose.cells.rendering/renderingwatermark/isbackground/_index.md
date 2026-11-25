---
title: "RenderingWatermark.IsBackground"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RenderingWatermark. Indica se la filigrana è posizionata dietro i contenuti della pagina"
type: docs
url: /it/net/aspose.cells.rendering/renderingwatermark/isbackground/
---
## RenderingWatermark.IsBackground property

Indica se la filigrana è posizionata dietro i contenuti della pagina.

```csharp
public bool IsBackground { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyIsBackgroundDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Sample Content");

            // Crea una filigrana con IsBackground impostato su true
            RenderingFont font = new RenderingFont("Arial", 36)
            {
                Color = Color.LightGray
            };
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
            {
                IsBackground = true,
                Rotation = 45,
                Opacity = 0.2f
            };

            // Configura le opzioni di salvataggio con filigrana
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Salva con filigrana di sfondo
            workbook.Save("WatermarkIsBackgroundDemo.pdf", options);
        }
    }
}
```

### Vedi anche

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


