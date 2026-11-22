---
title: "ChartArea.WidthRatioToChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartArea. تحصل أو تعين الإزاحة الأفقية من العمود السفلي الأيمن بوحدات نسبة مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartarea/widthratiotochart/
---
## ChartArea.WidthRatioToChart property

يحصل أو يضبط الإزاحة الأفقية من عمود الزاوية السفلية اليمنى، بوحدات نسبة من منطقة المخطط.

```csharp
public override double WidthRatioToChart { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyWidthRatioToChartDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // حساب المخطط
            chart.Calculate();

            // عرض خاصية WidthRatioToChart
            Console.WriteLine("Chart Area Width Ratio: " + chart.ChartArea.WidthRatioToChart);
            
            // تعديل النسبة وعرض التغيير
            chart.ChartArea.WidthRatioToChart = 0.8;
            Console.WriteLine("Modified Chart Area Width Ratio: " + chart.ChartArea.WidthRatioToChart);
        }
    }
}
```

### انظر أيضًا

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


