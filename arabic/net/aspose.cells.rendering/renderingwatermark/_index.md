---
title: "الفئة RenderingWatermark"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Rendering.RenderingWatermark. علامة مائية للتصيير"
type: docs
url: /ar/net/aspose.cells.rendering/renderingwatermark/
---
## RenderingWatermark class

علامة مائية للعرض.

```csharp
public class RenderingWatermark
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [RenderingWatermark](renderingwatermark/#constructor)(byte[]) | ينشئ كائنًا من العلامة المائية الصورة. |
| [RenderingWatermark](renderingwatermark/#constructor_1)(string, RenderingFont) | ينشئ كائنًا من العلامة المائية النصية. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Font](../../aspose.cells.rendering/renderingwatermark/font/) { get; } | يحصل على خط العلامة المائية. |
| [HAlignment](../../aspose.cells.rendering/renderingwatermark/halignment/) { get; set; } | يحصل أو يضبط محاذاة العلامة المائية الأفقية إلى الصفحة. |
| [Image](../../aspose.cells.rendering/renderingwatermark/image/) { get; } | يحصل على صورة العلامة المائية. |
| [IsBackground](../../aspose.cells.rendering/renderingwatermark/isbackground/) { get; set; } | يشير إلى ما إذا كانت العلامة المائية موضوعة خلف محتويات الصفحة. |
| [OffsetX](../../aspose.cells.rendering/renderingwatermark/offsetx/) { get; set; } | يحصل أو يضبط قيمة الإزاحة إلى [`HAlignment`](./halignment/) |
| [OffsetY](../../aspose.cells.rendering/renderingwatermark/offsety/) { get; set; } | يحصل أو يضبط قيمة الإزاحة إلى [`VAlignment`](./valignment/) |
| [Opacity](../../aspose.cells.rendering/renderingwatermark/opacity/) { get; set; } | يحصل أو يضبط شفافية العلامة المائية في النطاق [0, 1]. |
| [Rotation](../../aspose.cells.rendering/renderingwatermark/rotation/) { get; set; } | يحصل أو يضبط دوران العلامة المائية بالدرجات. |
| [ScaleToPagePercent](../../aspose.cells.rendering/renderingwatermark/scaletopagepercent/) { get; set; } | يحصل أو يضبط مقياس العلامة المائية نسبة إلى الصفحة المستهدفة بالنسبة المئوية. |
| [Text](../../aspose.cells.rendering/renderingwatermark/text/) { get; } | يحصل على نص العلامة المائية. |
| [VAlignment](../../aspose.cells.rendering/renderingwatermark/valignment/) { get; set; } | يحصل أو يضبط محاذاة العلامة المائية العمودية إلى الصفحة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class RenderingWatermarkDemo
    {
        public static void RenderingWatermarkExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample worksheet.");

            // إنشاء خط للعلامة المائية
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // إنشاء علامة مائية من النص والخط المحدد
            RenderingWatermark watermark = new RenderingWatermark("Watermark", font);

            // تعيين خصائص العلامة المائية
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 30;
            watermark.Opacity = 0.6f;
            watermark.ScaleToPagePercent = 50;
            watermark.IsBackground = true;

            // تحديد علامة مائية للتصيير إلى PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // احفظ المصنف كملف PDF مع العلامة المائية
            workbook.Save("output_watermark.pdf", options);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


