---
title: "MsoFormatPicture.BottomCropInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "MsoFormatPicture property. يمثل موقع الجزء السفلي من مستطيل القص معبرًا عنه بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells.drawing/msoformatpicture/bottomcropinch/
---
## MsoFormatPicture.BottomCropInch property

يمثل موضع الجزء السفلي من مستطيل القص، بوحدة البوصة.

```csharp
public double BottomCropInch { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyBottomCropInchDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف صورة إلى ورقة العمل (باستخدام مسار نائب)
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // الوصول إلى كائن MsoFormatPicture
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // حدد خاصية BottomCropInch ووضح استخدامها
            formatPicture.BottomCropInch = 0.3;
            formatPicture.TopCropInch = 0.2;
            
            // احفظ المصنف
            workbook.Save("MsoFormatPictureBottomCropDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


