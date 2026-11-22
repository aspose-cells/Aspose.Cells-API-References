---
title: "Picture.OriginalWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Picture. تحصل على العرض الأصلي للصورة"
type: docs
url: /ar/net/aspose.cells.drawing/picture/originalwidth/
---
## Picture.OriginalWidth property

تحصل على العرض الأصلي للصورة.

```csharp
public int OriginalWidth { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صورة إلى ورقة العمل
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[imgIndex];

            // احصل على العرض الأصلي للصورة وعرضه
            int originalWidth = pic.OriginalWidth;
            Console.WriteLine("Original width of the picture: " + originalWidth + " pixels");

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


