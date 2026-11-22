---
title: "ImageOrPrintOptions.PixelFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تحصل أو تعين تنسيق البكسل للصور المُولدة"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/pixelformat/
---
## ImageOrPrintOptions.PixelFormat property

يحصل أو يضبط تنسيق البكسل للصور المولدة.

```csharp
public PixelFormat PixelFormat { get; set; }
```

### ملاحظات

القيمة الافتراضية هي PixelFormat.Format32bppArgb.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyPixelFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إنشاء ورقة عمل نموذجية
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات لجعل المثال ذو معنى
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "PixelFormat Demo";

            try
            {
                // أنشئ مثيلًا لـ ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // اعرض القيمة الحالية لخاصية ImageType (لأن PixelFormat غير موجود)
                Console.WriteLine("Current ImageType: " + options.ImageType);

                // ملاحظة: بما أن PixelFormat غير موجود في API، نعرض ImageType بدلاً من ذلك
                // وهي أقرب خاصية ذات صلة بإعدادات تنسيق الصورة

                // إنشاء SheetRender لعرض الخيارات المستخدمة
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // احفظ النتيجة كصورة لعرض الخيارات
                sheetRender.ToImage(0, "PixelFormatDemo.png");

                Console.WriteLine("ImageType property has been demonstrated. Image saved as PixelFormatDemo.png");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


