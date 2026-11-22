---
title: "Title.YRatioToChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Title. تحصل أو تعين إحداثي y للزاوية العلوية اليسرى بوحدات جزء من مساحة المخطط. Y بالبكسل  YRatioToChart  Chart.ChartObject.Width"
type: docs
url: /ar/net/aspose.cells.charts/title/yratiotochart/
---
## Title.YRatioToChart property

يحصل أو يضبط إحداثي y للزاوية العلوية اليسرى بوحدات جزء من مساحة المخطط. Y بالبكسل = YRatioToChart * Chart.ChartObject.Width;

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

    public class TitlePropertyYRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على عنوان المخطط
            chart.Title.Text = "Sample Chart Title";
            Title chartTitle = chart.Title;

            // عرض قيمة YRatioToChart الحالية
            Console.WriteLine("Current YRatioToChart value: " + chartTitle.YRatioToChart);

            // غيّر خاصية YRatioToChart لتحريك العنوان عموديًا
            chartTitle.YRatioToChart = 0.1; // 10% from the top of the chart area
            Console.WriteLine("New YRatioToChart value: " + chartTitle.YRatioToChart);

            // احفظ المصنف
            workbook.Save("TitlePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


