---
title: "ShapePath.PathSegementList"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapePath. يحصل على قائمة ShapeSegmentPathCollection"
type: docs
url: /ar/net/aspose.cells.drawing/shapepath/pathsegementlist/
---
## ShapePath.PathSegementList property

يحصل على قائمة [`ShapeSegmentPathCollection`](../../shapesegmentpathcollection/)

```csharp
[Obsolete("Use ShapePath.PathSegments property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ShapeSegmentPathCollection PathSegementList { get; }
```

### ملاحظات

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية ShapePath.PathSegments. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyPathSegementListDemo
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

                Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("ShapePathPropertyPathSegementListDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapeSegmentPathCollection](../../shapesegmentpathcollection/)
* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


