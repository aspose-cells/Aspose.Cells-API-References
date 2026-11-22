---
title: "MsoFormatPicture.RightCropInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoFormatPicture. تمثل موقع الجانب الأيمن لمستطيل القص معبرًا عنه بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells.drawing/msoformatpicture/rightcropinch/
---
## MsoFormatPicture.RightCropInch property

يمثل موضع الجانب الأيمن من مستطيل القص، بوحدة البوصة.

```csharp
public double RightCropInch { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyRightCropInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف صورة (استبدل بمسار الصورة الفعلي)
            int pictureIndex = sheet.Pictures.Add(1, 1, "sample.jpg");
            Aspose.Cells.Drawing.Picture picture = sheet.Pictures[pictureIndex];

            // الوصول إلى خاصية RightCropInch وضبطها
            Aspose.Cells.Drawing.MsoFormatPicture format = picture.FormatPicture;
            format.RightCropInch = 0.3; // Crop 0.3 inches from right

            // احفظ المصنف
            workbook.Save("RightCropInchDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


