---
title: "ScrollBar.Min"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ScrollBar. تحصل أو تعيين القيمة الدنيا لشريط التمرير أو نطاق المؤشر"
type: docs
url: /ar/net/aspose.cells.drawing/scrollbar/min/
---
## ScrollBar.Min property

يحصل أو يضبط القيمة الدنيا لنطاق شريط التمرير أو المؤشر.

```csharp
public int Min { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyMinDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شريط تمرير إلى ورقة العمل
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // تعيين خصائص شريط التمرير
            scrollBar.Min = 10;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;  // Changed from Value to CurrentValue
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;

            // عرض قيمة خاصية Min
            Console.WriteLine("ScrollBar Min Value: " + scrollBar.Min);

            // احفظ المصنف
            workbook.Save("ScrollBarMinDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


