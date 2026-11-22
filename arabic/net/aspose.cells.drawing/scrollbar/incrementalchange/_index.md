---
title: "ScrollBar.IncrementalChange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ScrollBar. تحصل أو تعين مقدار الزيادة التي يتم تطبيقها على شريط التمرير أو المؤشر عند تمرير سطر واحد"
type: docs
url: /ar/net/aspose.cells.drawing/scrollbar/incrementalchange/
---
## ScrollBar.IncrementalChange property

يحصل أو يضبط مقدار الزيادة التي يضيفها شريط التمرير أو المؤشر عند تمرير سطر.

```csharp
public int IncrementalChange { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyIncrementalChangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شريط تمرير إلى ورقة العمل
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // تعيين خصائص شريط التمرير
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;
            scrollBar.IncrementalChange = 5; // This is the key property we're demonstrating
            scrollBar.PageChange = 20;

            // عرض خصائص شريط التمرير
            Console.WriteLine("Scroll Bar Properties:");
            Console.WriteLine("Min: " + scrollBar.Min);
            Console.WriteLine("Max: " + scrollBar.Max);
            Console.WriteLine("Current Value: " + scrollBar.CurrentValue);
            Console.WriteLine("Incremental Change: " + scrollBar.IncrementalChange);
            Console.WriteLine("Page Change: " + scrollBar.PageChange);

            // تعديل الزيادة المتدرجة
            scrollBar.IncrementalChange = 10;
            Console.WriteLine("\nModified Incremental Change: " + scrollBar.IncrementalChange);

            // احفظ المصنف
            workbook.Save("ScrollBarDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


