---
title: "Picture.OriginalHeight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Picture. تحصل على الارتفاع الأصلي للصورة"
type: docs
url: /ar/net/aspose.cells.drawing/picture/originalheight/
---
## Picture.OriginalHeight property

تحصل على الارتفاع الأصلي للصورة.

```csharp
public int OriginalHeight { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalHeightDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صورة إلى ورقة العمل
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];

            // احصل على وعرض الارتفاع الأصلي للصورة
            int originalHeight = pic.OriginalHeight;
            Console.WriteLine("Original height of the picture: " + originalHeight + " pixels");

            // احفظ المصنف
            workbook.Save("result.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


