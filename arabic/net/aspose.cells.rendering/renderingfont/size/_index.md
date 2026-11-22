---
title: "RenderingFont.Size"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RenderingFont. يحصل على حجم الخط بالنقاط"
type: docs
url: /ar/net/aspose.cells.rendering/renderingfont/size/
---
## RenderingFont.Size property

يحصل على حجم الخط بالنقاط.

```csharp
public float Size { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingFontPropertySizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // إنشاء الخط الأولي وإظهار قراءة خاصية Size
            RenderingFont smallFont = new RenderingFont("Arial", 12);
            Console.WriteLine("Initial font size: " + smallFont.Size);

            // إنشاء علامة مائية بحجم الخط الأولي
            PdfSaveOptions optionsSmall = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", smallFont)
            };
            workbook.Save("SmallWatermark.pdf", optionsSmall);

            // إنشاء خط جديد بحجم أكبر
            RenderingFont largeFont = new RenderingFont("Arial", 24);
            Console.WriteLine("Modified font size: " + largeFont.Size);

            // إنشاء علامة مائية بحجم خط أكبر
            PdfSaveOptions optionsLarge = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", largeFont)
            };
            workbook.Save("LargeWatermark.pdf", optionsLarge);
        }
    }
}
```

### انظر أيضًا

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


