---
title: "Shape.RelativeToOriginalPictureSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تشير إلى ما إذا كان الشكل نسبياً إلى حجم الصورة الأصلي"
type: docs
url: /ar/net/aspose.cells.drawing/shape/relativetooriginalpicturesize/
---
## Shape.RelativeToOriginalPictureSize property

يشير إلى ما إذا كان الشكل نسبياً إلى حجم الصورة الأصلي.

```csharp
public bool RelativeToOriginalPictureSize { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRelativeToOriginalPictureSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صورة إلى ورقة العمل
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];

            // الوصول إلى خصائص الشكل - الصورة هي بالفعل Shape، لا حاجة للتحويل
            Shape shape = picture;

            // إظهار خاصية RelativeToOriginalPictureSize
            Console.WriteLine("Original RelativeToOriginalPictureSize: " + shape.RelativeToOriginalPictureSize);
            
            // تغيير الخاصية
            shape.RelativeToOriginalPictureSize = !shape.RelativeToOriginalPictureSize;
            Console.WriteLine("Modified RelativeToOriginalPictureSize: " + shape.RelativeToOriginalPictureSize);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


