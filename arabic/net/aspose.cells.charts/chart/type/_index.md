---
title: "Chart.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية المخطط. تحصل أو تعيّن نوع المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chart/type/
---
## Chart.Type property

يحصل على أو يضبط نوع المخطط.

```csharp
public ChartType Type { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // أضف مخطط رادار
            int chartIndex = sheet.Charts.Add(ChartType.Radar, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // توضيح استخدام خاصية Type
            Console.WriteLine("Chart type is: " + chart.Type);
            
            // غيّر نوع المخطط إلى عمود
            chart.Type = ChartType.Column;
            Console.WriteLine("Chart type changed to: " + chart.Type);
        }
    }
}
```

### انظر أيضًا

* enum [ChartType](../../charttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


