---
title: "ListBox.PageChange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListBox. تحدد مقدار التغيير في قيمة التحكم عندما ينقر المستخدم على منطقة صفحة أعلى أو صفحة أسفل في أشرطة التمرير"
type: docs
url: /ar/net/aspose.cells.drawing/listbox/pagechange/
---
## ListBox.PageChange property

يحدد مقدار تغيير قيمة التحكم عندما ينقر المستخدم على منطقة الصفحة للأعلى أو للأسفل في شريط التمرير.

```csharp
public int PageChange { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertyPageChangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل ListBox
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(1, 0, 1, 0, 100, 100);

            // تعيين بعض العناصر لـ ListBox
            listBox.SetInputRange("A1:A5", false, false);
            
            // تعيين خاصية PageChange
            listBox.PageChange = 2;

            // احفظ المصنف
            workbook.Save("ListBoxPageChangeDemo.xlsx");

            // عرض قيمة PageChange
            Console.WriteLine("ListBox PageChange value: " + listBox.PageChange);
        }
    }
}
```

### انظر أيضًا

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


