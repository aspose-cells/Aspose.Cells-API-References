---
title: "PictureCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PictureCollection. يحصل على عنصر Picture عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/picturecollection/item/
---
## PictureCollection indexer

يحصل على عنصر [`Picture`](../../picture/) عند الفهرس المحدد.

```csharp
public Picture this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الحصول على مجموعة الصور
            PictureCollection pictures = worksheet.Pictures;
            
            // إضافة صورة (استبدل "image.png" بالمسار الفعلي للصورة)
            int index = pictures.Add(1, 1, "image.png");
            
            // الوصول إلى الصورة باستخدام خاصية Item
            Picture pic = pictures[index];
            
            // عرض استخدام خاصية Item
            Console.WriteLine($"Picture at index {index} has width: {pic.Width} and height: {pic.Height}");
            
            // تعديل خصائص الصورة
            pic.Height = 200;
            pic.Width = 300;
            
            // احفظ المصنف
            workbook.Save("PictureCollectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Picture](../../picture/)
* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


