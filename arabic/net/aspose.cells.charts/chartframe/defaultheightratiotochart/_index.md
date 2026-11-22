---
title: "ChartFrame.DefaultHeightRatioToChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تمثل ارتفاع الموضع الافتراضي بوحدات نسبة مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/defaultheightratiotochart/
---
## ChartFrame.DefaultHeightRatioToChart property

يمثل ارتفاع الموضع الافتراضي بوحدات جزء من مساحة المخطط.

```csharp
public double DefaultHeightRatioToChart { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultHeightRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى عنوان المخطط (الذي هو ChartFrame)
            ChartFrame chartTitle = chart.Title;

            // عرض قيمة DefaultHeightRatioToChart الحالية
            Console.WriteLine("Current DefaultHeightRatioToChart value: " + chartTitle.DefaultHeightRatioToChart);

            // إظهار كيف تؤثر هذه الخاصية على المخطط بالمقارنة مع HeightRatioToChart
            Console.WriteLine("Current HeightRatioToChart value: " + chartTitle.HeightRatioToChart);

            // غيّر نسبة الارتفاع لرؤية التأثير
            chartTitle.HeightRatioToChart = 0.1;
            Console.WriteLine("After setting HeightRatioToChart to 0.1: " + chartTitle.HeightRatioToChart);

            // احفظ المصنف
            workbook.Save("ChartFramePropertyDefaultHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


