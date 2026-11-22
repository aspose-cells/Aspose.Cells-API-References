---
title: "ShapeCollection.AddLabel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تُضيف Label إلى ورقة العمل"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addlabel/
---
## ShapeCollection.AddLabel method

يضيف Label إلى ورقة العمل.

```csharp
public Label AddLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| أعلى | Int32 | يمثل الإزاحة العمودية لـ Label من الصف الأيسر، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| يسار | Int32 | يمثل الإزاحة الأفقية لـ Label من العمود الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | يمثل ارتفاع Label، بوحدة البكسل. |
| العرض | Int32 | يمثل عرض Label، بوحدة البكسل. |

### قيمة الإرجاع

كائن Label.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLabelWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على مجموعة الأشكال
            ShapeCollection shapes = worksheet.Shapes;

            // أضف label إلى ورقة العمل
            Label label = shapes.AddLabel(1, 0, 1, 0, 100, 50);
            label.Text = "Sample Label";

            // احفظ المصنف
            workbook.Save("AddLabelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


