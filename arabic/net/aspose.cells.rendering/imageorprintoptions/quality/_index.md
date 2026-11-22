---
title: "ImageOrPrintOptions.Quality"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تحصل أو تعيين قيمة تحدد جودة الصور المُنشأة لتُطبق فقط عند حفظ الصفحات بتنسيق Jpeg. القيمة الافتراضية هي 100"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/quality/
---
## ImageOrPrintOptions.Quality property

يحصل أو يضبط قيمة تحدد جودة الصور المولدة لتُطبق فقط عند حفظ الصفحات بتنسيق `Jpeg`. القيمة الافتراضية هي 100

```csharp
public int Quality { get; set; }
```

### ملاحظات

يؤثر فقط عند الحفظ بصيغة JPEG. يجب أن تكون القيمة بين 0 و 100. القيمة الافتراضية هي 100.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyQualityDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["C3"].PutValue(DateTime.Now);

            // إنشاء خيارات الصورة بإعدادات جودة مختلفة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;
            options.Quality = 100; // Highest quality

            // تحويل ورقة العمل إلى صورة بجودة عالية
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "HighQualityOutput.jpg");

            // تغيير الجودة لتوضيح الفرق
            options.Quality = 50; // Medium quality
            renderer.ToImage(0, "MediumQualityOutput.jpg");

            options.Quality = 10; // Low quality
            renderer.ToImage(0, "LowQualityOutput.jpg");
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


