---
title: "ShapePathCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapePathCollection. تحصل على مسار إنشاء"
type: docs
url: /ar/net/aspose.cells.drawing/shapepathcollection/item/
---
## ShapePathCollection indexer

يحصل على مسار الإنشاء.

```csharp
public ShapePath this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### قيمة الإرجاع

يعيد كائن [`ShapePath`](../../shapepath/)

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePathCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مخصصًا (شكل غير بدائي) مع المعلمات الصحيحة
            Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 10, 10, 200, 200, 0, 0);

            // الوصول إلى ShapePathCollection
            ShapePathCollection shapePaths = customShape.Paths;

            // أضف مسارًا جديدًا
            int pathIndex = shapePaths.Add();

            // الوصول إلى المسار باستخدام خاصية Item
            ShapePath newPath = shapePaths[pathIndex];

            // إخراج المعلومات
            Console.WriteLine("Path count: " + shapePaths.Count);
            Console.WriteLine("Path segment count: " + newPath.PathSegementList.Count);

            // احفظ المصنف
            workbook.Save("ShapePathCollectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapePath](../../shapepath/)
* class [ShapePathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


