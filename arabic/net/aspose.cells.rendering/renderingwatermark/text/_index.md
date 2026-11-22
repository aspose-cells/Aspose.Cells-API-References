---
title: "RenderingWatermark.Text"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RenderingWatermark. تحصل على نص العلامة المائية"
type: docs
url: /ar/net/aspose.cells.rendering/renderingwatermark/text/
---
## RenderingWatermark.Text property

يحصل على نص العلامة المائية.

```csharp
public string Text { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingWatermarkPropertyTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء خط عرض للنص العلامة المائية
            RenderingFont font = new RenderingFont("Arial", 36);

            // تهيئة علامة مائية نصية باستخدام تكوين الخط
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);

            // عرض نص العلامة المائية الحالي
            Console.WriteLine("Watermark Text: " + watermark.Text);

            // تكوين مظهر العلامة المائية
            watermark.Rotation = 45f;
            watermark.Opacity = 0.3f;
            watermark.IsBackground = true;
            watermark.ScaleToPagePercent = 150;

            // تطبيق العلامة المائية على خيارات حفظ PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark; // Fixed property name

            // حفظ إلى PDF لتصور تأثيرات العلامة المائية
            workbook.Save("WatermarkDemo.pdf", options);
        }
    }
}
```

### انظر أيضًا

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


