---
title: "Series.HasDropLines"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. True إذا كان المخطط يحتوي على خطوط إسقاط. ينطبق فقط على المخططات الخطية أو مخططات المنطقة"
type: docs
url: /ar/net/aspose.cells.charts/series/hasdroplines/
---
## Series.HasDropLines property

صحيح إذا كان للمخطط خطوط سقوط. ينطبق فقط على المخطط الخطي أو مخططات المساحة.

```csharp
public bool HasDropLines { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasDropLinesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط خطي
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة بيانات السلسلة
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على السلسلة الأولى
            Series series = chart.NSeries[0];

            // إظهار خاصية HasDropLines
            series.HasDropLines = true; // Enable drop lines
            series.Type = ChartType.Line; // Ensure it's a line chart for drop lines to be visible

            // احفظ المصنف
            workbook.Save("SeriesHasDropLinesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


