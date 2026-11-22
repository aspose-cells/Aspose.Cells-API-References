---
title: "RenderingWatermark.OffsetY"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RenderingWatermark. تحصل أو تعين قيمة الإزاحة إلى VAlignment"
type: docs
url: /ar/net/aspose.cells.rendering/renderingwatermark/offsety/
---
## RenderingWatermark.OffsetY property

تحصل أو تعين قيمة الإزاحة إلى [`VAlignment`](../valignment/)

```csharp
public float OffsetY { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyOffsetYDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("OffsetY Demo");

            // أنشئ خط العلامة المائية
            RenderingFont font = new RenderingFont("Arial", 24)
            {
                Color = Color.Red,
                Bold = true
            };

            // إنشاء علامة مائية بقيم OffsetY مختلفة
            RenderingWatermark watermark = new RenderingWatermark("VERTICAL OFFSET", font)
            {
                Rotation = 0,
                Opacity = 0.3f,
                IsBackground = true,
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                OffsetX = 0,
                OffsetY = 100 // Demonstrating OffsetY property
            };

            // تعيين خيارات الحفظ مع علامة مائية
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // حفظ مع إزاحة العلامة المائية
            workbook.Save("WatermarkOffsetYDemo.pdf", options);
        }
    }
}
```

### انظر أيضًا

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


