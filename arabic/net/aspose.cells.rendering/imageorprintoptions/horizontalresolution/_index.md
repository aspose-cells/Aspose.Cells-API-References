---
title: "ImageOrPrintOptions.HorizontalResolution"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تحصل أو تعين الدقة الأفقية للصور المولدة بالنقطة في البوصة"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/horizontalresolution/
---
## ImageOrPrintOptions.HorizontalResolution property

يحصل أو يضبط الدقة الأفقية للصور المولدة، بوحدة النقاط في البوصة.

```csharp
public int HorizontalResolution { get; set; }
```

### ملاحظات

القيمة الافتراضية هي 96.

ضبط `HorizontalResolution` و[`VerticalResolution`](../verticalresolution/) يؤثر على عرض وارتفاع الصورة الناتجة بالبكسل.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyHorizontalResolutionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text for Image Rendering");

            // تهيئة ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            
            // تعيين الدقة الأفقية والعمودية
            options.HorizontalResolution = 192;
            options.VerticalResolution = 192;

            // تحويل ورقة العمل إلى صورة بالدقة المحددة
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "WorksheetImage_192dpi.png");

            // توضيح دقة مختلفة
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;
            renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "WorksheetImage_300dpi.png");
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


