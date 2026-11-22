---
title: "Picture.SourceFullName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Picture. تحصل أو تعين المسار والاسم لملف المصدر للصورة المرتبطة"
type: docs
url: /ar/net/aspose.cells.drawing/picture/sourcefullname/
---
## Picture.SourceFullName property

يحصل على أو يضبط المسار واسم ملف المصدر للصورة المرتبطة.

```csharp
public string SourceFullName { get; set; }
```

### ملاحظات

القيمة الافتراضية هي سلسلة فارغة. إذا لم يكن SourceFullName سلسلة فارغة، فإن الصورة مرتبطة. إذا لم يكن SourceFullName سلسلة فارغة، ولكن Data يساوي null، فإن الصورة تكون مرتبطة ولا تُخزن في الملف.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertySourceFullNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صورة مرتبطة إلى ورقة العمل
            string imagePath = "example.png";
            Picture picture = worksheet.Shapes.AddLinkedPicture(0, 0, 100, 100, imagePath);

            // عرض خاصية SourceFullName
            Console.WriteLine("Picture SourceFullName: " + picture.SourceFullName);
            Console.WriteLine("Is linked picture: " + picture.IsLink);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


