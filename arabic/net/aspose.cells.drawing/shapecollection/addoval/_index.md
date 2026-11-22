---
title: "ShapeCollection.AddOval"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تضيف Oval إلى ورقة العمل"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addoval/
---
## ShapeCollection.AddOval method

يضيف Oval إلى ورقة العمل.

```csharp
public Oval AddOval(int topRow, int top, int leftColumn, int left, int height, int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| أعلى | Int32 | يمثل الإزاحة العمودية لـ Oval من الصف الأيسر، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| يسار | Int32 | يمثل الإزاحة الأفقية لـ Oval من العمود الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | يمثل ارتفاع Oval، بوحدة البكسل. |
| العرض | Int32 | يمثل عرض Oval، بوحدة البكسل. |

### قيمة الإرجاع

كائن Oval.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddOvalWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً بيضاويًا إلى ورقة العمل
            ShapeCollection shapes = worksheet.Shapes;
            Oval oval = shapes.AddOval(1, 0, 1, 0, 50, 50);

            // احفظ المصنف
            workbook.Save("AddOvalDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Oval](../../oval/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


