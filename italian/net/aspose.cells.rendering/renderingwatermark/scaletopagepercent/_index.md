---
title: "RenderingWatermark.ScaleToPagePercent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RenderingWatermark. Ottiene o imposta la scala relativa alla pagina di destinazione in percentuale"
type: docs
url: /it/net/aspose.cells.rendering/renderingwatermark/scaletopagepercent/
---
## RenderingWatermark.ScaleToPagePercent property

Ottiene o imposta la scala relativa alla pagina di destinazione in percentuale.

```csharp
public int ScaleToPagePercent { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyScaleToPagePercentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample worksheet with watermark");

            RenderingFont font = new RenderingFont("Arial", 72);
            font.Bold = true;
            font.Color = Color.LightBlue;

            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            watermark.ScaleToPagePercent = 75;
            watermark.Opacity = 0.3f;
            watermark.IsBackground = true;

            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            workbook.Save("WatermarkDemo.pdf", options);
        }
    }
}
```

### Vedi anche

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


