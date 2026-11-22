---
title: "ChartFrame.IsAutomaticSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تشير إلى ما إذا كان إطار المخطط مُحَدَّدًا تلقائيًا"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/isautomaticsize/
---
## ChartFrame.IsAutomaticSize property

يشير إلى ما إذا كان حجم إطار المخطط يتم ضبطه تلقائيًا.

```csharp
public virtual bool IsAutomaticSize { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyIsAutomaticSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى legend وإظهار خاصية IsAutomaticSize
            Aspose.Cells.Charts.Legend legend = chart.Legend;
            
            // اضبط الحجم التلقائي إلى false وإظهار القيمة
            legend.IsAutomaticSize = false;
            Console.WriteLine("Legend Automatic Size: " + legend.IsAutomaticSize);
            
            // اضبط الحجم التلقائي إلى true وإظهار القيمة
            legend.IsAutomaticSize = true;
            Console.WriteLine("Legend Automatic Size: " + legend.IsAutomaticSize);
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


