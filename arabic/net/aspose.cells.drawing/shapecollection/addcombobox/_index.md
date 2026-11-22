---
title: "ShapeCollection.AddComboBox"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تضيف ComboBox إلى ورقة العمل"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addcombobox/
---
## ShapeCollection.AddComboBox method

يضيف ComboBox إلى ورقة العمل.

```csharp
public ComboBox AddComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| أعلى | Int32 | يمثل الإزاحة العمودية لComboBox من الصف الأيسر، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| يسار | Int32 | يمثل الإزاحة الأفقية لComboBox من العمود الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | يمثل ارتفاع ComboBox، بوحدة البكسل. |
| العرض | Int32 | يمثل عرض ComboBox، بوحدة البكسل. |

### قيمة الإرجاع

كائن ComboBox.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddComboBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على مجموعة الأشكال
            ShapeCollection shapes = worksheet.Shapes;

            // أضف مربع اختيار مع المعلمات المحددة
            Aspose.Cells.Drawing.ComboBox comboBox = shapes.AddComboBox(1, 0, 1, 0, 100, 50);

            // أضف عناصر إلى مربع الاختيار عن طريق تعيين قيم الخلايا
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // تعيين نطاق الإدخال لمربع القائمة
            comboBox.InputRange = "A1:A3";
            comboBox.DropDownLines = 3;

            // احفظ المصنف
            workbook.Save("AddComboBoxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ComboBox](../../combobox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


