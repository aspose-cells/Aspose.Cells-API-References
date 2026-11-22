---
title: "MsoFormatPicture.RightCrop"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "MsoFormatPicture property. يمثل موقع الجانب الأيمن من مستطيل القص معبرًا عنه كنسبة من عرض الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/msoformatpicture/rightcrop/
---
## MsoFormatPicture.RightCrop property

يمثل موضع الجانب الأيمن من مستطيل القص، معبرًا عنه كنسبة من عرض الصورة.

```csharp
public double RightCrop { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPicturePropertyRightCropDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صورة إلى ورقة العمل
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];
            
            // احصل على MsoFormatPicture للصورة
            MsoFormatPicture msoFormatPicture = picture.FormatPicture;

            // اعرض القيمة الحالية لـ RightCrop
            Console.WriteLine("Current RightCrop value: " + msoFormatPicture.RightCrop);

            // حدد قيمة RightCrop جديدة (0.2 يعني قص 20٪ من اليمين)
            msoFormatPicture.RightCrop = 0.2;
            Console.WriteLine("New RightCrop value set to: " + msoFormatPicture.RightCrop);

            // حفظ المصنف لرؤية التأثير
            workbook.Save("RightCropDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


