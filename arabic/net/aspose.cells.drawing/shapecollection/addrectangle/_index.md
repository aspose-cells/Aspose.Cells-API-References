---
title: "ShapeCollection.AddRectangle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تضيف RectangleShape إلى ورقة العمل"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addrectangle/
---
## ShapeCollection.AddRectangle method

يضيف RectangleShape إلى ورقة العمل.

```csharp
public RectangleShape AddRectangle(int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| أعلى | Int32 | يمثل الإزاحة العمودية لـ RectangleShape من صفه الأيسر، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| يسار | Int32 | يمثل الإزاحة الأفقية لـ RectangleShape من العمود الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | يمثل ارتفاع RectangleShape، بوحدة البكسل. |
| العرض | Int32 | يمثل عرض RectangleShape، بوحدة البكسل. |

### قيمة الإرجاع

كائن RectangleShape.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddRectangleWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف مستطيلًا باستخدام المعلمات المحددة
            RectangleShape rectangleShape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // احفظ المصنف
            workbook.Save("RectangleShapeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [RectangleShape](../../rectangleshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


