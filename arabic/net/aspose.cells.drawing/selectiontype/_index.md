---
title: "تعداد SelectionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.SelectionType. نوع التحديد لصندوق القائمة"
type: docs
url: /ar/net/aspose.cells.drawing/selectiontype/
---
## SelectionType enumeration

نوع الاختيار لصندوق القائمة.

```csharp
public enum SelectionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Single | `0` | نوع التحديد الفردي. |
| Multi | `1` | نوع اختيار متعدد. |
| Extend | `2` | توسيع نوع الاختيار. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassSelectionTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع قائمة إلى ورقة العمل
            ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 5, 10);

            // تعيين نوع الاختيار إلى فردي
            listBox.SelectionType = SelectionType.Single;

            // إضافة عناصر إلى مربع القائمة
            listBox.SetInputRange("A1:A5", false, false);

            // تحقق من نوع الاختيار
            Console.WriteLine("ListBox SelectionType: " + listBox.SelectionType);

            // احفظ المصنف
            workbook.Save("SelectionTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


