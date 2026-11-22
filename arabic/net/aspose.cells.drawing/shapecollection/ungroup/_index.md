---
title: "ShapeCollection.Ungroup"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تفك تجميع عناصر الشكل."
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/ungroup/
---
## ShapeCollection.Ungroup method

فك تجميع عناصر الشكل.

```csharp
public void Ungroup(GroupShape group)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تجميع | GroupShape | شكل التجميع. |

### ملاحظات

إذا كان شكل التجميع مُجَمَّعًا بواسطة شكل تجميع آخر، لن يتم تنفيذ أي شيء.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodUngroupWithGroupShapeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على مجموعة الأشكال
            ShapeCollection shapes = worksheet.Shapes;

            // إضافة الشكل المستطيل الأول
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // إضافة الشكل المستطيل الثاني
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // إنشاء مصفوفة من الأشكال للتجميع
            Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };

            // اجمع الأشكال
            GroupShape groupShape = shapes.Group(shapesArr);

            // فك تجميع شكل التجميع
            shapes.Ungroup(groupShape);
        }
    }
}
```

### انظر أيضًا

* class [GroupShape](../../groupshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


