---
title: "فئة RenderingFont"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Rendering.RenderingFont. خط للعرض"
type: docs
url: /ar/net/aspose.cells.rendering/renderingfont/
---
## RenderingFont class

الخط للعرض.

```csharp
public class RenderingFont
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [RenderingFont](renderingfont/)(string, float) | ينشئ مثيلًا جديدًا لـ `RenderingFont` |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Bold](../../aspose.cells.rendering/renderingfont/bold/) { get; set; } | يحصل أو يعيّن السُمك العريض للخط. |
| [Color](../../aspose.cells.rendering/renderingfont/color/) { get; set; } | يحصل أو يعيّن اللون للخط. |
| [Italic](../../aspose.cells.rendering/renderingfont/italic/) { get; set; } | يحصل أو يعيّن الخط المائل للخط. |
| [Name](../../aspose.cells.rendering/renderingfont/name/) { get; } | يحصل على اسم الخط. |
| [Size](../../aspose.cells.rendering/renderingfont/size/) { get; } | يحصل على حجم الخط بالنقاط. |

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontDemo
    {
        public static void RenderingFontExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            sheet.Cells["A1"].PutValue("Hello World!");

            // إنشاء كائن RenderingFont
            RenderingFont renderingFont = new RenderingFont("Arial", 12)
            {
                Bold = true,
                Italic = true,
                Color = Color.Blue
            };

            // إنشاء كائن RenderingWatermark باستخدام RenderingFont
            RenderingWatermark watermark = new RenderingWatermark("Sample Watermark", renderingFont)
            {
                Rotation = 45,
                ScaleToPagePercent = 100,
                Opacity = 0.5f,
                IsBackground = true,
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                OffsetX = 0,
                OffsetY = 0
            };

            // إنشاء PdfSaveOptions وتعيين العلامة المائية
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions
            {
                Watermark = watermark,
                EmbedStandardWindowsFonts = true,
                CalculateFormula = true,
                ExportDocumentStructure = true,
                DisplayDocTitle = true
            };

            // حفظ المصنف إلى PDF مع العلامة المائية
            workbook.Save("RenderingFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


