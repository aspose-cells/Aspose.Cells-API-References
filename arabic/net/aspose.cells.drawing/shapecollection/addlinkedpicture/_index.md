---
title: "ShapeCollection.AddLinkedPicture"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. إضافة صورة مرتبطة"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addlinkedpicture/
---
## ShapeCollection.AddLinkedPicture method

أضف صورة مرتبطة.

```csharp
public Picture AddLinkedPicture(int topRow, int leftColumn, int height, int width, 
    string sourceFullName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| الارتفاع | Int32 | ارتفاع الشكل. بوحدة البكسل |
| العرض | Int32 | عرض الشكل. بوحدة البكسل |
| sourceFullName | String | المسار واسم ملف المصدر للصورة المرتبطة |

### قيمة الإرجاع

[`Picture`](../../picture/) Picture object.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLinkedPictureWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة نص تجريبي إلى الخلية A1
            worksheet.Cells["A1"].PutValue("Image will be linked below:");
            
            // إضافة صورة مرتبطة إلى ورقة العمل
            string imageUrl = "https://example.com/sample.jpg";
            worksheet.Shapes.AddLinkedPicture(1, 1, 100, 100, imageUrl);
            
            // احفظ المصنف
            workbook.Save("output_with_linked_picture.xlsx");
            
            Console.WriteLine("Workbook saved with linked picture.");
        }
    }
}
```

### انظر أيضًا

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


