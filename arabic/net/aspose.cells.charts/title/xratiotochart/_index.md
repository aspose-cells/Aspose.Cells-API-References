---
title: "Title.XRatioToChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Title. تحصل أو تعين إحداثي x للزاوية العلوية اليسرى بوحدات جزء من مساحة المخطط. X بالبكسل  XRatioToChart  Chart.ChartObject.Width"
type: docs
url: /ar/net/aspose.cells.charts/title/xratiotochart/
---
## Title.XRatioToChart property

يحصل أو يضبط إحداثي x للزاوية العلوية اليسرى بوحدات جزء من مساحة المخطط. X بالبكسل = XRatioToChart * Chart.ChartObject.Width;

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

    public class TitlePropertyXRatioToChartDemo
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

            // اضبط مصدر البيانات للمخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على عنوان المخطط
            chart.Title.Text = "Sample Chart Title";
            Title title = chart.Title;

            // اعرض قيمة XRatioToChart الحالية
            Console.WriteLine("Current XRatioToChart value: " + title.XRatioToChart);

            // غيّر قيمة XRatioToChart لتحريك العنوان أفقيًا
            title.XRatioToChart = 0.25; // 25% from the left of the chart area
            Console.WriteLine("New XRatioToChart value: " + title.XRatioToChart);

            // احفظ المصنف
            workbook.Save("TitlePropertyXRatioToChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


