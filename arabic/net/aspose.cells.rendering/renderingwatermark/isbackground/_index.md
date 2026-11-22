---
title: "RenderingWatermark.IsBackground"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RenderingWatermark. تشير إلى ما إذا كانت العلامة المائية موضوعة خلف محتويات الصفحة"
type: docs
url: /ar/net/aspose.cells.rendering/renderingwatermark/isbackground/
---
## RenderingWatermark.IsBackground property

يشير إلى ما إذا كانت العلامة المائية موضوعة خلف محتويات الصفحة.

```csharp
public bool IsBackground { get; set; }
```

### أمثلة

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
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Sample Content");

            // إنشاء علامة مائية مع تعيين IsBackground إلى true
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

            // تكوين خيارات الحفظ مع العلامة المائية
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // حفظ مع علامة مائية خلفية
            workbook.Save("WatermarkIsBackgroundDemo.pdf", options);
        }
    }
}
```

### انظر أيضًا

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


