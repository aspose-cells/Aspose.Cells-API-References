---
title: "RenderingWatermark.Font"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RenderingWatermark. تحصل على خط العلامة المائية"
type: docs
url: /ar/net/aspose.cells.rendering/renderingwatermark/font/
---
## RenderingWatermark.Font property

يحصل على خط العلامة المائية.

```csharp
public RenderingFont Font { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingWatermarkPropertyFontDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إنشاء خط عرض وتعيين الخصائص الأولية
            RenderingFont font = new RenderingFont("Arial", 24);
            
            // إنشاء علامة مائية نصية بخط العرض
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            
            // عرض خصائص الخط الأولية
            Console.WriteLine("Initial Font Name: " + watermark.Font.Name);
            Console.WriteLine("Initial Font Size: " + watermark.Font.Size);
            Console.WriteLine("Initial Bold Status: " + watermark.Font.Bold);
            
            // تعديل خصائص الخط عبر مرجع RenderingFont
            font.Bold = true;
            
            // عرض خصائص الخط المحدثة من العلامة المائية
            Console.WriteLine("\nUpdated Font Name: " + watermark.Font.Name);
            Console.WriteLine("Updated Font Size: " + watermark.Font.Size);
            Console.WriteLine("Updated Bold Status: " + watermark.Font.Bold);
            
            // تكوين خصائص عرض العلامة المائية
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            watermark.IsBackground = true;
            
            // إنشاء خيارات حفظ PDF وتعيين العلامة المائية
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Watermark = watermark;
            
            // حفظ المصنف بملف PDF مع علامة مائية لإظهار تغييرات الخط
            workbook.Save("RenderingWatermarkFontDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### انظر أيضًا

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


