---
title: "MsoFormatPicture.BottomCrop"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "MsoFormatPicture property. يمثل موقع الجزء السفلي من مستطيل القص معبرًا عنه كنسبة من ارتفاع الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/msoformatpicture/bottomcrop/
---
## MsoFormatPicture.BottomCrop property

يمثل موضع الجزء السفلي من مستطيل القص، معبرًا عنه كنسبة من ارتفاع الصورة.

```csharp
public double BottomCrop { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPicturePropertyBottomCropDemo
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

            // اعرض القيمة الحالية لـ BottomCrop
            Console.WriteLine("Current BottomCrop value: " + msoFormatPicture.BottomCrop);

            // حدد قيمة BottomCrop جديدة (0.2 يعني قص 20٪ من الأسفل)
            msoFormatPicture.BottomCrop = 0.2;
            Console.WriteLine("BottomCrop set to: " + msoFormatPicture.BottomCrop);

            // حدد قيم قص أخرى لتوضيح التأثير
            msoFormatPicture.TopCrop = 0.1;
            msoFormatPicture.LeftCrop = 0.1;
            msoFormatPicture.RightCrop = 0.1;

            // احفظ المصنف لرؤية الصورة المقصوصة
            workbook.Save("MsoFormatPicturePropertyBottomCropDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


