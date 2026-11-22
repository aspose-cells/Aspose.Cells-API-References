---
title: "ShapeCollection.DeleteShape"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. حذف شكل. إذا كان الشكل داخل مجموعة أو كان شكل تعليق فلن يتم حذفه"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/deleteshape/
---
## ShapeCollection.DeleteShape method

احذف شكلاً. إذا كان الشكل في مجموعة أو كان شكلاً تعليقًا، فلن يتم حذفه.

```csharp
public void DeleteShape(Shape shape)
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
    public class ShapeCollectionMethodDeleteShapeWithShapeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على مجموعة الأشكال
            ShapeCollection shapes = worksheet.Shapes;

            // إضافة الشكل المستطيل الأول
            Shape firstShape = shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // إضافة الشكل المستطيل الثاني
            Shape secondShape = shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // حذف الشكل الأول
            shapes.DeleteShape(firstShape);

            // احفظ المصنف
            workbook.Save("DeleteShapeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


