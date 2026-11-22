---
title: "RenderingFont.Bold"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RenderingFont. يحصل أو يعيّن الخط العريض للخط"
type: docs
url: /ar/net/aspose.cells.rendering/renderingfont/bold/
---
## RenderingFont.Bold property

يحصل أو يعيّن السُمك العريض للخط.

```csharp
public bool Bold { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontPropertyBoldDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Bold Font Example");

            // إنشاء نمط للخلية
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            worksheet.Cells["A1"].SetStyle(style);

            // إنشاء خيارات حفظ PDF مع علامة مائية تُظهر الخط العريض
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // إنشاء خط عرض مع خاصية عريضة
            RenderingFont font = new RenderingFont("Arial", 36)
            {
                Bold = true,
                Color = System.Drawing.Color.Red
            };
            
            // إنشاء علامة مائية بخط عريض
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Opacity = 0.3f
            };
            pdfSaveOptions.Watermark = watermark;

            // احفظ المصنف
            workbook.Save("BoldFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### انظر أيضًا

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


