---
title: "RenderingWatermark.ScaleToPagePercent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RenderingWatermark. Obtient ou définit l'échelle relative à la page cible en pourcentage"
type: docs
url: /fr/net/aspose.cells.rendering/renderingwatermark/scaletopagepercent/
---
## RenderingWatermark.ScaleToPagePercent property

Obtient ou définit l'échelle relative à la page cible en pourcentage.

```csharp
public int ScaleToPagePercent { get; set; }
```

### Exemples

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

### Voir aussi

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


