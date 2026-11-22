---
title: "ChartFrame.WidthRatioToChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تحصل أو تعين عرض الإطار بوحدات نسبة من مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/widthratiotochart/
---
## ChartFrame.WidthRatioToChart property

يحصل على أو يضبط عرض الإطار بوحدات نسبة مساحة المخطط.

```csharp
public virtual double WidthRatioToChart { get; set; }
```

### ملاحظات

هذه قيمة كسرية، نطاقها الصالح بين 0-1. كيف يتم تحويل وحدات النسبة إلى بكسل؟ WidthPixel = WidthRatioToChart * Chart.ChartObject.Width;

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyWidthRatioToChartDemo
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

            // عرض نسبة العرض الحالية
            Console.WriteLine("Current WidthRatioToChart value: " + chartTitle.WidthRatioToChart);

            // تعيين نسبة عرض جديدة (0.5 = 50% من عرض المخطط)
            chartTitle.WidthRatioToChart = 0.5;

            // عرض التأثير عن طريق حفظ المصنف
            workbook.Save("ChartFrameWidthRatioDemo.xlsx");

            Console.WriteLine("WidthRatioToChart property demonstrated successfully.");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


