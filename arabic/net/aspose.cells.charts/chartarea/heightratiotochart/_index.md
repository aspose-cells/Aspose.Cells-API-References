---
title: "ChartArea.HeightRatioToChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartArea. تحصل أو تعين الإزاحة العمودية من صف الزاوية السفلية اليمنى بوحدات نسبة مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartarea/heightratiotochart/
---
## ChartArea.HeightRatioToChart property

يحصل أو يضبط الإزاحة العمودية من صف الزاوية السفلية اليمنى، بوحدات نسبة من منطقة المخطط.

```csharp
public override double HeightRatioToChart { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyHeightRatioToChartDemo
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

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // الوصول إلى منطقة المخطط
            ChartArea chartArea = chart.ChartArea;

            // اعرض قيمة HeightRatioToChart الحالية
            Console.WriteLine("Current HeightRatioToChart value: " + chartArea.HeightRatioToChart);

            // عيّن قيمة جديدة لـ HeightRatioToChart (0.5 = 50٪ من ارتفاع المخطط)
            chartArea.HeightRatioToChart = 0.5;
            Console.WriteLine("New HeightRatioToChart value: " + chartArea.HeightRatioToChart);

            // عيّن قيمة جديدة لـ WidthRatioToChart لتوضيح التأثير المشترك
            chartArea.WidthRatioToChart = 0.8;

            // احفظ المصنف لرؤية التغييرات
            workbook.Save("ChartAreaPropertyHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


