---
title: "PictureCollection.RemoveAt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PictureCollection. إزالة الأشكال عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/picturecollection/removeat/
---
## PictureCollection.RemoveAt method

إزالة الأشكال عند الفهرس المحدد

```csharp
public void RemoveAt(int index)
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض الصور إلى ورقة العمل
            int index1 = worksheet.Pictures.Add(1, 1, "image1.png");
            int index2 = worksheet.Pictures.Add(5, 1, "image2.png");
            int index3 = worksheet.Pictures.Add(10, 1, "image3.png");

            Console.WriteLine("Number of pictures before removal: " + worksheet.Pictures.Count);

            // إزالة الصورة عند الفهرس المحدد
            worksheet.Pictures.RemoveAt(index2);

            Console.WriteLine("Number of pictures after removal: " + worksheet.Pictures.Count);
        }
    }
}
```

### انظر أيضًا

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


