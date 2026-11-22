---
title: "MsoFormatPicture.Brightness"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoFormatPicture. تمثل تعديل السطوع للصورة بوحدة النسبة المئوية"
type: docs
url: /ar/net/aspose.cells.drawing/msoformatpicture/brightness/
---
## MsoFormatPicture.Brightness property

يمثل تعديل السطوع للصورة بوحدة النسبة المئوية.

```csharp
public double Brightness { get; set; }
```

### ملاحظات

إنها بين -100% و 100%. تعمل بنفس طريقة Excel 2007 أو الإصدارات الأحدث.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyBrightnessDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صورة إلى ورقة العمل
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[pictureIndex];

            // تعيين والحصول على السطوع
            picture.FormatPicture.Brightness = 30;
            Console.WriteLine("Picture brightness: " + picture.FormatPicture.Brightness);

            // تعديل السطوع
            picture.FormatPicture.Brightness = 70;
            Console.WriteLine("Updated brightness: " + picture.FormatPicture.Brightness);
        }
    }
}
```

### انظر أيضًا

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


