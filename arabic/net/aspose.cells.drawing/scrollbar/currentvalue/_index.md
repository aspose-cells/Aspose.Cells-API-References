---
title: "ScrollBar.CurrentValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ScrollBar. تحصل أو تعيين القيمة الحالية"
type: docs
url: /ar/net/aspose.cells.drawing/scrollbar/currentvalue/
---
## ScrollBar.CurrentValue property

يحصل أو يضبط القيمة الحالية.

```csharp
public int CurrentValue { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyCurrentValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شريط تمرير إلى ورقة العمل
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // تعيين خصائص شريط التمرير باستخدام أسماء الخصائص الصحيحة
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;

            // تعيين وعرض خاصية CurrentValue
            scrollBar.CurrentValue = 50;
            Console.WriteLine("ScrollBar CurrentValue: " + scrollBar.CurrentValue);

            // تغيير القيمة الحالية
            scrollBar.CurrentValue = 75;
            Console.WriteLine("Updated ScrollBar CurrentValue: " + scrollBar.CurrentValue);

            // احفظ المصنف
            workbook.Save("ScrollBarCurrentValueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


