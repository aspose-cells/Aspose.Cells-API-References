---
title: "ScrollBar.Shadow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ScrollBar. تشير إلى ما إذا كان الشكل يحتوي على تظليل ثلاثي الأبعاد"
type: docs
url: /ar/net/aspose.cells.drawing/scrollbar/shadow/
---
## ScrollBar.Shadow property

يشير إلى ما إذا كان الشكل يحتوي على تظليل ثلاثي الأبعاد.

```csharp
public bool Shadow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyShadowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شريط تمرير أفقي
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);
            
            // تعيين خصائص شريط التمرير
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;
            scrollBar.CurrentValue = 50;
            scrollBar.IsHorizontal = true;
            
            // عرض خاصية Shadow
            scrollBar.Shadow = true; // Enable 3D shadow effect
            
            // إنشاء شريط تمرير آخر للمقارنة
            ScrollBar scrollBar2 = worksheet.Shapes.AddScrollBar(1, 2, 1, 1, 100, 20);
            scrollBar2.Shadow = false; // No shadow
            
            // احفظ المصنف
            workbook.Save("ScrollBarShadowDemo.xlsx");
            
            Console.WriteLine("ScrollBar Shadow demo completed. Check output file.");
        }
    }
}
```

### انظر أيضًا

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


