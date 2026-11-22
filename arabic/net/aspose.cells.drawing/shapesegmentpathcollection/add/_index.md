---
title: "ShapeSegmentPathCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeSegmentPathCollection. أضف مسار مقطع في مسار الإنشاء"
type: docs
url: /ar/net/aspose.cells.drawing/shapesegmentpathcollection/add/
---
## ShapeSegmentPathCollection.Add method

أضف مسار مقطع في مسار الإنشاء.

```csharp
public int Add(ShapePathType type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | ShapePathType | نوع المسار. |

### قيمة الإرجاع

يرجع موضع [`ShapeSegmentPath`](../../shapesegmentpath/) الكائن في القائمة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathCollectionMethodAddWithShapePathTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ShapePath path = new ShapePath();

            // ابدأ مسارًا جديدًا
            path.MoveTo(10, 10);

            // ارسم مقطع خط
            path.LineTo(100, 100);

            // الوصول إلى خاصية PathSegementList
            ShapeSegmentPathCollection segmentList = path.PathSegementList;

            segmentList.Add(ShapePathType.Close);

            // عرض عدد مقاطع المسار
            Console.WriteLine("Number of path segments: " + segmentList.Count);

            // التكرار عبر كل مقطع وعرض نوعه
            foreach (ShapeSegmentPath segment in segmentList)
            {
                Console.WriteLine("Segment type: " + segment.Type);
            }

           
            //إضافة شكل حر
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

            // احفظ المصنف لملاحظة تعديلات الشكل
            workbook.Save("ShapeSegmentPathCollectionAddDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


