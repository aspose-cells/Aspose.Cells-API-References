---
title: "PdfSaveOptions.Watermark"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSaveOptions. تحصل أو تعيّن العلامة المائية للإخراج"
type: docs
url: /ar/net/aspose.cells/pdfsaveoptions/watermark/
---
## PdfSaveOptions.Watermark property

يحصل على أو يضبط العلامة المائية للإخراج.

```csharp
public RenderingWatermark Watermark { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyWatermarkDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا يحتوي على 3 أوراق عمل
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells["A1"].PutValue("Page1");
            int index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page2");
            index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page3");

            // أنشئ خط العلامة المائية
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // أنشئ علامة مائية بالنص والخط
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 45;
            watermark.Opacity = 0.3f;
            watermark.ScaleToPagePercent = 75;

            // عيّن العلامة المائية في خيارات حفظ PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // احفظ المصنف مع العلامة المائية
            wb.Save("output_watermark.pdf", options);
        }
    }
}
```

### انظر أيضًا

* class [RenderingWatermark](../../../aspose.cells.rendering/renderingwatermark/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


