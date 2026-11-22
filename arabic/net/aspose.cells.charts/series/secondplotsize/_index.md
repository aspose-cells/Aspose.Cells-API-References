---
title: "Series.SecondPlotSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية السلسلة. تُرجع أو تُعيّن حجم القسم الثانوي إما في مخطط فطيرة داخل فطيرة أو شريط داخل فطيرة كنسبة مئوية من حجم الفطيرة الأساسية. يمكن أن تكون قيمة من 5 إلى 200"
type: docs
url: /ar/net/aspose.cells.charts/series/secondplotsize/
---
## Series.SecondPlotSize property

يعيد أو يضبط حجم القسم الثانوي إما في مخطط فطيرة داخل فطيرة أو شريط داخل فطيرة، كنسبة مئوية من حجم الفطيرة الأساسية. يمكن أن يكون قيمة من 5 إلى 200.

```csharp
public short SecondPlotSize { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySecondPlotSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة لمخطط الفطيرة
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // إضافة مخطط فطيرة
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على السلسلة الأولى
            Series series = chart.NSeries[0];

            // تعيين خاصية SecondPlotSize (نسبة مئوية للفطيرة لتظهر في المخطط الثانوي)
            series.SecondPlotSize = 30; // 30% of the pie will be shown in second plot

            // احفظ المصنف
            workbook.Save("SeriesPropertySecondPlotSizeDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


