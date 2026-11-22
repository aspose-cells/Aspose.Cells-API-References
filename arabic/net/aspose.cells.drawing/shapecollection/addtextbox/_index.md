---
title: "ShapeCollection.AddTextBox"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. يضيف مربع نص إلى ورقة العمل"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addtextbox/
---
## ShapeCollection.AddTextBox method

يضيف مربع نص إلى ورقة العمل.

```csharp
public TextBox AddTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| أعلى | Int32 | يمثل الإزاحة العمودية لمربع النص من صفه العلوي، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| يسار | Int32 | يمثل الإزاحة الأفقية لمربع النص من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | يمثل ارتفاع مربع النص، بوحدة البكسل. |
| العرض | Int32 | يمثل عرض مربع النص، بوحدة البكسل. |

### قيمة الإرجاع

كائن [`TextBox`](../../textbox/).

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على مجموعة الأشكال
            ShapeCollection shapes = worksheet.Shapes;

            // أضف مربع نص مع الموضع والحجم المحددين
            TextBox textBox = shapes.AddTextBox(1, 0, 1, 0, 100, 50);
            textBox.Text = "Sample TextBox";

            // احفظ المصنف
            workbook.Save("TextBoxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


