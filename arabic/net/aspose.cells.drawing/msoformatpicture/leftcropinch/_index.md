---
title: "MsoFormatPicture.LeftCropInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoFormatPicture. تمثل موقع الجانب الأيسر لمستطيل القص معبرًا عنه بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells.drawing/msoformatpicture/leftcropinch/
---
## MsoFormatPicture.LeftCropInch property

يمثل موضع الجانب الأيسر من مستطيل القص، بوحدة البوصة.

```csharp
public double LeftCropInch { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyLeftCropInchDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            var workbook = new Workbook();
            var sheet = workbook.Worksheets[0];

            // تحميل بيانات الصورة
            byte[] imageData = File.ReadAllBytes("example.png");
            
            // إضافة صورة إلى ورقة العمل
            int pictureIndex = sheet.Pictures.Add(0, 0, new MemoryStream(imageData));
            var picture = sheet.Pictures[pictureIndex];

            // اضبط واحصل على خاصية LeftCropInch
            picture.FormatPicture.LeftCropInch = 0.5;
            double leftCropValue = picture.FormatPicture.LeftCropInch;

            Console.WriteLine($"Left crop value in inches: {leftCropValue}");

            // احفظ المصنف
            workbook.Save("LeftCropInchDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


