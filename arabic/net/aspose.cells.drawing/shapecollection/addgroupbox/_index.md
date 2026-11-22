---
title: "ShapeCollection.AddGroupBox"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. يضيف GroupBox إلى ورقة العمل"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addgroupbox/
---
## ShapeCollection.AddGroupBox method

يضيف GroupBox إلى ورقة العمل.

```csharp
public GroupBox AddGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| أعلى | Int32 | يمثل الإزاحة العمودية لـ GroupBox من صفه الأيسر، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| يسار | Int32 | يمثل الإزاحة الأفقية لـ GroupBox من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | يمثل ارتفاع GroupBox، بوحدة البكسل. |
| العرض | Int32 | يمثل عرض GroupBox، بوحدة البكسل. |

### قيمة الإرجاع

كائن GroupBox.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddGroupBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة GroupBox إلى ورقة العمل
            ShapeCollection shapes = worksheet.Shapes;
            Aspose.Cells.Drawing.GroupBox groupBox = shapes.AddGroupBox(1, 0, 1, 0, 100, 50);

            // احفظ المصنف
            workbook.Save("GroupBoxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [GroupBox](../../groupbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


