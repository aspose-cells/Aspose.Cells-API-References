---
title: "ChartArea.XRatioToChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartArea. تحصل أو تعين الإزاحة الأفقية من العمود العلوي الأيسر كنسبة من مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartarea/xratiotochart/
---
## ChartArea.XRatioToChart property

يحصل أو يضبط الإزاحة الأفقية من عمود الزاوية العليا اليسرى، كنسبة من منطقة المخطط.

```csharp
public override double XRatioToChart { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyXRatioToChartDemo
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

            // احصل على مساحة المخطط
            ChartArea chartArea = chart.ChartArea;

            // عرض القيمة الحالية لـ XRatioToChart
            Console.WriteLine("Current XRatioToChart value: " + chartArea.XRatioToChart);

            // تغيير قيمة XRatioToChart لتحريك مساحة المخطط أفقياً
            chartArea.XRatioToChart = 0.2; // 20% from the left of the chart container

            // عرض القيمة الجديدة لـ XRatioToChart
            Console.WriteLine("New XRatioToChart value: " + chartArea.XRatioToChart);

            // احفظ المصنف
            workbook.Save("ChartAreaXRatioToChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


