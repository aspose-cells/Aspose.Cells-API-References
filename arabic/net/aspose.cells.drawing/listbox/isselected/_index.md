---
title: "ListBox.IsSelected"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ListBox. تشير إلى ما إذا كان العنصر محددًا"
type: docs
url: /ar/net/aspose.cells.drawing/listbox/isselected/
---
## ListBox.IsSelected method

يشير إلى ما إذا كان العنصر محددًا.

```csharp
public bool IsSelected(int itemIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| itemIndex | Int32 | فهرس العنصر. |

### قيمة الإرجاع

ما إذا كان العنصر محددًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxMethodIsSelectedWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع قائمة إلى ورقة العمل
            ListBox listBox = worksheet.Shapes.AddListBox(0, 0, 100, 100, 200, 200);

            // تعيين عناصر القائمة عبر نطاق الخلايا المرتبط
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            listBox.LinkedCell = "A1:A3";

            // حدد عنصرًا
            listBox.SelectedIndex = 0;

            // تحقق من حالة الاختيار باستخدام IsSelected مع معامل Int32
            Console.WriteLine("Item 0 selected: " + listBox.IsSelected(0));
            Console.WriteLine("Item 1 selected: " + listBox.IsSelected(1));
            Console.WriteLine("Item 2 selected: " + listBox.IsSelected(2));
        }
    }
}
```

### انظر أيضًا

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


