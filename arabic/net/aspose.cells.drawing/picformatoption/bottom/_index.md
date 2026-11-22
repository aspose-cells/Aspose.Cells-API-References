---
title: "PicFormatOption.Bottom"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PicFormatOption. تحصل أو تعين الإزاحة السفلية لتمديد الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/picformatoption/bottom/
---
## PicFormatOption.Bottom property

يحصل أو يضبط الإزاحة السفلية لتمديد الصورة.

```csharp
public double Bottom { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyBottomDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // استخدم ملف صورة موجود (استبدله بمسار الصورة الفعلي)
            string imagePath = "sample.jpg";

            // أضف شكلاً مستطيلًا إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);

            // قم بتكوين تعبئة الشكل لاستخدام الصورة النموذجية
            // يتم استنتاج FillType عند تعيين ImageData، مما يحدد النوع إلى Texture
            shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);
            
            // إنشاء وتكوين خيارات تنسيق الصورة
            PicFormatOption picFormat = new PicFormatOption();
            picFormat.Type = FillPictureType.Stretch;

            // عرض القيمة الأولية لـ Bottom
            Console.WriteLine("Initial Bottom value: " + picFormat.Bottom);

            // عدّل إزاحة Bottom وعرض القيمة الجديدة
            picFormat.Bottom = 0.3;
            Console.WriteLine("Modified Bottom value: " + picFormat.Bottom);

            // اربط PicFormatOption بتعبئة الشكل (بافتراض القابلية للتطبيق)
            // ملاحظة: قد يتطلب هذه الخطوة طرقًا خاصة بـ API غير معروضة في السياق المقدم
            // للتوضيح، تم إنشاء PicFormatOption وتكوينه

            // احفظ المصنف مع التغييرات المطبقة
            workbook.Save("PicFormatOptionBottomDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


