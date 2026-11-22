---
title: "ShapeSegmentPath.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapeSegmentPath. يحصل على نوع مقطع المسار"
type: docs
url: /ar/net/aspose.cells.drawing/shapesegmentpath/type/
---
## ShapeSegmentPath.Type property

يحصل على نوع جزء المسار

```csharp
public ShapePathType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //إنشاء مسار شكل جديد
                ShapePath shapePath = new ShapePath();

                // الانتقال إلى النقطة البداية
                shapePath.MoveTo(10, 10);

                // استدعاء طريقة LineTo مع معلمات (Single, Single)
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                // الوصول إلى خاصية PathSegementList
                ShapeSegmentPathCollection segmentList = shapePath.PathSegementList;

                // عرض عدد مقاطع المسار
                Console.WriteLine("Number of path segments: " + segmentList.Count);

                // التكرار عبر كل مقطع وعرض نوعه
                foreach (ShapeSegmentPath segment in segmentList)
                {
                    Console.WriteLine("Segment type: " + segment.Type);
                }

                //إضافة شكل حر
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }


            // احفظ المصنف
            workbook.Save("ShapeSegmentPathTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


