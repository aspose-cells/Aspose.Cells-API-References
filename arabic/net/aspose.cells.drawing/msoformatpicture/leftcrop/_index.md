---
title: "MsoFormatPicture.LeftCrop"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoFormatPicture. تمثل موقع اليسار لمستطيل القص معبرًا عنه كنسبة من عرض الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/msoformatpicture/leftcrop/
---
## MsoFormatPicture.LeftCrop property

يمثل موضع الجانب الأيسر من مستطيل القص، معبرًا عنه كنسبة من عرض الصورة.

```csharp
public double LeftCrop { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyLeftCropDemo
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

            // تعيين خاصية LeftCrop
            picture.FormatPicture.LeftCrop = 0.1;
            Console.WriteLine("LeftCrop set to: " + picture.FormatPicture.LeftCrop);

            // الحصول على خاصية LeftCropInch وتعيينها
            double leftCropInch = picture.FormatPicture.LeftCropInch;
            picture.FormatPicture.LeftCropInch = leftCropInch;
            Console.WriteLine("LeftCropInch value: " + leftCropInch);

            // احفظ المصنف
            workbook.Save("LeftCropDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


