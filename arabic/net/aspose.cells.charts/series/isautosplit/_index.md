---
title: "Series.IsAutoSplit"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. تُشير إلى ما إذا كانت قيمة العتبة تلقائية"
type: docs
url: /ar/net/aspose.cells.charts/series/isautosplit/
---
## Series.IsAutoSplit property

يشير إلى ما إذا كانت قيمة العتبة تلقائية.

```csharp
public bool IsAutoSplit { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsAutoSplitDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["A5"].PutValue("Grape");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // إضافة مخطط فطيرة
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // الوصول إلى السلسلة الأولى وعرض خاصية IsAutoSplit
            Series series = chart.NSeries[0];
            bool isAutoSplit = series.IsAutoSplit; // Get the value instead of setting it
            series.SplitValue = 25; // Split at value 25

            Console.WriteLine($"IsAutoSplit value: {isAutoSplit}");

            // احفظ المصنف
            workbook.Save("SeriesPropertyIsAutoSplitDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


