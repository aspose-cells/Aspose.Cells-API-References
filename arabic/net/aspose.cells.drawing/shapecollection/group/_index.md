---
title: "ShapeCollection.Group"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تجميع الأشكال"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/group/
---
## ShapeCollection.Group method

اجمع الأشكال في مجموعة.

```csharp
public GroupShape Group(Shape[] groupItems)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| groupItems | Shape[] | عناصر المجموعة. |

### قيمة الإرجاع

يعيد شكل المجموعة.

### ملاحظات

يجب ألا يكون الشكل في groupItems مُجمّعًا. يجب أن يكون الشكل في مجموعة Shapes هذه.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodGroupWithShapeArrayDemo
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

            // إنشاء مصفوفة تحتوي على الأشكال لتجميعها
            Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };

            // اجمع الأشكال
            GroupShape groupShape = shapes.Group(shapesArr);

            // احفظ المصنف
            workbook.Save("GroupShapesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [GroupShape](../../groupshape/)
* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


