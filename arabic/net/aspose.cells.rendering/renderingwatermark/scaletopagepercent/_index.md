---
title: "RenderingWatermark.ScaleToPagePercent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RenderingWatermark. تحصل أو تعين المقياس نسبةً إلى الصفحة المستهدفة بالنسبة المئوية"
type: docs
url: /ar/net/aspose.cells.rendering/renderingwatermark/scaletopagepercent/
---
## RenderingWatermark.ScaleToPagePercent property

يحصل أو يضبط مقياس العلامة المائية نسبة إلى الصفحة المستهدفة بالنسبة المئوية.

```csharp
public int ScaleToPagePercent { get; set; }
```

### أمثلة

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

### انظر أيضًا

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


