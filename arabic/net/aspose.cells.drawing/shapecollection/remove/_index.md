---
title: "ShapeCollection.Remove"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. إزالة الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/remove/
---
## ShapeCollection.Remove method

أزل الشكل.

```csharp
public void Remove(Shape shape)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| شكل | شكل |  |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodRemoveWithShapeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على مجموعة الأشكال
            ShapeCollection shapes = worksheet.Shapes;

            // إضافة الشكل المستطيل الأول
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            // إضافة الشكل المستطيل الثاني
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // احصل على الشكل الأول بالاسم أو الفهرس
            Shape shapeToRemove = shapes["Rectangle 1"]; // or shapes[0];
            
            if (shapeToRemove != null)
            {
                // إزالة الشكل من المجموعة
                shapes.Remove(shapeToRemove);
            }

            // احفظ المصنف
            workbook.Save("ShapeRemoveDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


