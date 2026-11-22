---
title: "MsoFormatPicture.TopCrop"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoFormatPicture. تمثل موقع أعلى مستطيل القص معبرًا عنه كنسبة من ارتفاع الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/msoformatpicture/topcrop/
---
## MsoFormatPicture.TopCrop property

يمثل موضع الجزء العلوي من مستطيل القص، معبرًا عنه كنسبة من ارتفاع الصورة.

```csharp
public double TopCrop { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTopCropDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف صورة إلى ورقة العمل
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
            
            // تعيين خاصية TopCrop
            picture.FormatPicture.TopCrop = -6;
            
            // إخراج قيمة TopCrop
            Console.WriteLine("Picture TopCrop value: " + picture.FormatPicture.TopCrop);
            
            // احفظ المصنف
            workbook.Save("TopCropDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


