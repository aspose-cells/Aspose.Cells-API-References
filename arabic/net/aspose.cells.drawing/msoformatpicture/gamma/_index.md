---
title: "MsoFormatPicture.Gamma"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoFormatPicture. تمثل قيمة جاما للصورة"
type: docs
url: /ar/net/aspose.cells.drawing/msoformatpicture/gamma/
---
## MsoFormatPicture.Gamma property

يمثل قيمة غاما للصورة.

```csharp
public double Gamma { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyGammaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف صورة إلى ورقة العمل (باستخدام مسار صورة نموذجي)
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // الوصول إلى كائن MsoFormatPicture
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // تعيين خاصية Gamma
            formatPicture.Gamma = 1.5; // Demonstrating Gamma adjustment

            // احفظ المصنف
            workbook.Save("MsoFormatPictureGammaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


