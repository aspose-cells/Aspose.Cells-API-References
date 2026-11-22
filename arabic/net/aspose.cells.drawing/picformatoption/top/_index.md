---
title: "PicFormatOption.Top"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PicFormatOption. تحصل أو تعين الإزاحة العلوية لتمديد الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/picformatoption/top/
---
## PicFormatOption.Top property

يحصل أو يضبط الإزاحة العلوية لتمديد الصورة.

```csharp
public double Top { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyTopDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // استخدم صورة موجودة أو قدم مسار الصورة الصحيح
            string imagePath = "existingImage.png";

            // أضف شكلاً بالمعلمات الصحيحة
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
            
            // طبق تعبئة الصورة باستخدام ImageData
            shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);

            // إنشاء وتكوين PicFormatOption مباشرة
            PicFormatOption picFormat = new PicFormatOption();

            Console.WriteLine("Initial Top value: " + picFormat.Top);
            picFormat.Top = 0.3;

            // افتراض أن PicFormatOption يحتاج إلى الارتباط بتنسيق التعبئة
            // قد يتطلب هذا الجزء تنفيذًا خاصًا بـ API غير معروض في تعريفات الأنواع
            // shape.FillFormat.SetPicFormatOption(picFormat);

            Console.WriteLine("Modified Top value: " + picFormat.Top);
            workbook.Save("TopPropertyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


