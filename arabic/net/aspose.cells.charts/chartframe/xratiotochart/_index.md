---
title: "ChartFrame.XRatioToChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تحصل أو تضبط إحداثي x للزاوية العلوية اليسرى بوحدات نسبة مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/xratiotochart/
---
## ChartFrame.XRatioToChart property

يحصل على أو يضبط إحداثي x للزاوية العليا اليسرى بوحدات نسبة مساحة المخطط.

```csharp
public virtual double XRatioToChart { get; set; }
```

### ملاحظات

هذه قيمة كسرية، نطاقها الصالح بين 0-1. كيف يتم تحويل وحدات النسبة إلى بكسلات؟ XPixel = XRatioToChart * Chart.ChartObject.Width;

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyXRatioToChartDemo
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

            // الوصول إلى عنوان المخطط الذي هو ChartFrame
            ChartFrame chartTitle = chart.Title;

            // اعرض قيمة XRatioToChart الحالية
            Console.WriteLine("Current XRatioToChart value: " + chartTitle.XRatioToChart);

            // تعيين قيمة XRatioToChart جديدة (0.5 تعني 50% من عرض المخطط من اليسار)
            chartTitle.XRatioToChart = 0.5;

            // عرض الموضع الجديد
            Console.WriteLine("Title position after change - XRatioToChart: " + chartTitle.XRatioToChart);

            // احفظ المصنف
            workbook.Save("ChartFrameXRatioToChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


