---
title: "ShapeSegmentPathCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapeSegmentPathCollection. يحصل على كائن ShapeSegmentPath"
type: docs
url: /ar/net/aspose.cells.drawing/shapesegmentpathcollection/item/
---
## ShapeSegmentPathCollection indexer

يحصل على كائن [`ShapeSegmentPath`](../../shapesegmentpath/).

```csharp
public ShapeSegmentPath this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### قيمة الإرجاع

يرجع كائن [`ShapeSegmentPath`](../../shapesegmentpath/).

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathCollectionPropertyItemDemo
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
            ShapeSegmentPathCollection segmentPaths = path.PathSegementList;


            segmentPaths.Add(ShapePathType.Close);

            // عرض عدد مقاطع المسار
            Console.WriteLine("Number of path segments: " + segmentPaths.Count);
          
            
            // توضيح قراءة خاصية Item
            for (int i = 0; i < segmentPaths.Count; i++)
            {
                ShapeSegmentPath segment = segmentPaths[i];
                Console.WriteLine($"Segment {i} type: {segment.Type}");
            }

            //إضافة شكل حر
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });
            // احفظ المصنف
            workbook.Save("ShapeSegmentPathCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapeSegmentPath](../../shapesegmentpath/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


