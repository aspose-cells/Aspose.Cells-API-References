---
title: "ShapeCollection.AddRadioButton"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. يضيف زر اختيار إلى ورقة العمل"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addradiobutton/
---
## ShapeCollection.AddRadioButton method

يضيف RadioButton إلى ورقة العمل.

```csharp
public RadioButton AddRadioButton(int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| أعلى | Int32 | يمثل الإزاحة العمودية لزر الاختيار من صفه الأيسر، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| يسار | Int32 | يمثل الإزاحة الأفقية لRadioButton من العمود الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | يمثل ارتفاع RadioButton، بوحدة البكسل. |
| العرض | Int32 | يمثل عرض RadioButton، بوحدة البكسل. |

### قيمة الإرجاع

كائن RadioButton.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddRadioButtonWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة زر اختيار إلى ورقة العمل
            Aspose.Cells.Drawing.RadioButton radioButton = worksheet.Shapes.AddRadioButton(1, 0, 1, 0, 100, 50);
            radioButton.Text = "Option 1";

            // احفظ المصنف
            workbook.Save("RadioButtonDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [RadioButton](../../radiobutton/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


