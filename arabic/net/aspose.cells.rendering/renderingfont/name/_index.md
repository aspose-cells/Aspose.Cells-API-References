---
title: "RenderingFont.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RenderingFont. يحصل على اسم الخط"
type: docs
url: /ar/net/aspose.cells.rendering/renderingfont/name/
---
## RenderingFont.Name property

يحصل على اسم الخط.

```csharp
public string Name { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingFontPropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أنشئ خيارات حفظ PDF
            PdfSaveOptions options = new PdfSaveOptions();

            // إنشاء خط عرض أولي باستخدام "Arial"
            RenderingFont fontArial = new RenderingFont("Arial", 16);
            Console.WriteLine("Initial font name: " + fontArial.Name);

            // إنشاء علامة مائية بالخط الأولي
            RenderingWatermark watermark = new RenderingWatermark("Confidential", fontArial);
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            options.Watermark = watermark;

            // حفظ مع علامة مائية للخط الأولي
            workbook.Save("WatermarkInitial.pdf", options);

            // إنشاء خط عرض جديد باستخدام "Times New Roman"
            RenderingFont fontTimesNewRoman = new RenderingFont("Times New Roman", 16);
            Console.WriteLine("\nModified font name: " + fontTimesNewRoman.Name);

            // تحديث العلامة المائية بالخط الجديد
            RenderingWatermark updatedWatermark = new RenderingWatermark("Confidential", fontTimesNewRoman);
            updatedWatermark.Opacity = 0.5f;
            updatedWatermark.Rotation = 45;
            options.Watermark = updatedWatermark;

            // حفظ مع علامة مائية للخط المعدل
            workbook.Save("WatermarkModified.pdf", options);
        }
    }
}
```

### انظر أيضًا

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


