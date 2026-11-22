---
title: "ChartArea.YRatioToChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartArea. تحصل أو تحصل على الإزاحة العمودية من صف الزاوية العلوية اليسرى بوحدات نسبة مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartarea/yratiotochart/
---
## ChartArea.YRatioToChart property

يحصل أو يحصل على الإزاحة العمودية من صف الزاوية العليا اليسرى، بوحدات نسبة من منطقة المخطط.

```csharp
public override double YRatioToChart { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyYRatioToChartDemo
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
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى منطقة المخطط
            ChartArea chartArea = chart.ChartArea;

            // اعرض قيمة YRatioToChart الحالية
            Console.WriteLine("Current YRatioToChart value: " + chartArea.YRatioToChart);

            // غيّر خاصية YRatioToChart (0.0 إلى 1.0 تمثل 0٪ إلى 100٪ من مساحة المخطط)
            chartArea.YRatioToChart = 0.2; // Move chart area down by 20% of chart height

            // اعرض قيمة YRatioToChart الجديدة
            Console.WriteLine("New YRatioToChart value: " + chartArea.YRatioToChart);

            // حفظ المصنف لرؤية التأثير
            workbook.Save("ChartAreaPropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


