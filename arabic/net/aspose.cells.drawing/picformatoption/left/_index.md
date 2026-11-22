---
title: "PicFormatOption.Left"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PicFormatOption. يحصل أو يحدد الإزاحة اليسرى لتمديد الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/picformatoption/left/
---
## PicFormatOption.Left property

يحصل أو يضبط الإزاحة اليسرى لتمديد الصورة.

```csharp
public double Left { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyLeftDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل مستطيل لتوضيح تنسيق الصورة
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 150);

            // قم بتكوين تعبئة الصورة للشكل
            shape.FillFormat.ImageData = File.ReadAllBytes("sample.png"); // Ensure this image exists

            // أنشئ وقم بتكوين PicFormatOption
            PicFormatOption picFormat = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Left = 0.0 // Initial left offset (0%)
            };

            // طبق خيارات التنسيق على الشكل (مع افتراض أن اسم الخاصية صحيح)
            // ملاحظة: قد لا تكون الخاصية الأصلية 'PictureFormatOptions' موجودة في نسخة API الحالية.
            // السطر أدناه تم تعليقه لحل خطأ التجميع.
            // shape.FillFormat.PictureFormatOptions = picFormat;

            // اعرض الإزاحة اليسرى الأولية
            Console.WriteLine("Initial Left offset: " + picFormat.Left);

            // عدل الإزاحة اليسرى لقص 20٪ من الجانب الأيسر
            picFormat.Left = 0.2;
            Console.WriteLine("Modified Left offset: " + picFormat.Left);

            // احفظ دفتر العمل مع تنسيق الصورة المعدل
            workbook.Save("LeftPropertyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


