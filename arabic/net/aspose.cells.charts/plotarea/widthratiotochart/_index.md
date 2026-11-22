---
title: "PlotArea.WidthRatioToChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PlotArea. تحصّل أو تعين عرض صندوق الحدود لمنطقة الرسم بوحدات نسبة مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/plotarea/widthratiotochart/
---
## PlotArea.WidthRatioToChart property

يحصل أو يحدد عرض صندوق حدود مساحة الرسم بوحدات نسبة مساحة المخطط.

```csharp
public override double WidthRatioToChart { get; set; }
```

### ملاحظات

مربع حدود مساحة الرسم يشمل مساحة الرسم، علامات الفواصل (تسميات الفواصل)، وإطارًا صغيرًا حول علامات الفواصل. إذا لم يتم إنشاء القيمة بواسطة MS Excel، يرجى استدعاء طريقة Chart.Calculate() قبل استدعاء هذه الطريقة.

الـ **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** و **HeightRatioToChart** لـ **PlotArea** تمثل صندوق الحدود لمنطقة الرسم الذي يشمل منطقة الرسم، علامات الفواصل (تسميات الفواصل)، وحدود صغيرة حول علامات الفواصل. إذا كنت تريد الحصول على الحجم الفعلي لمنطقة الرسم، يجب عليك استدعاء خصائص **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** و **InnerHeightRatioToChart**.

بالنسبة إلى Excel 2007 أو أحدث، القيمة الافتراضية هي صفر. يجب عليك الحصول على القيمة بعد استدعاء Chart.Calculate().

WidthPixel = WidthRatioToChart * chart.ChartObject.Width. ملاحظة: عندما يتم تعيين WidthRatioToChart، سيتم تعيين خاصية IsInnerMode تلقائيًا إلى false.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyWidthRatioToChartDemo
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

            // أضف مخططًا واحصل على منطقة الرسم الخاصة به
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            PlotArea plotArea = chart.PlotArea;

            // عرض قيمة WidthRatioToChart الحالية
            Console.WriteLine("Current WidthRatioToChart value: " + plotArea.WidthRatioToChart);

            // غيّر نسبة العرض وشاهد التأثير
            plotArea.WidthRatioToChart = 0.6; // 60% of chart width
            Console.WriteLine("WidthRatioToChart changed to: " + plotArea.WidthRatioToChart);

            // احفظ المصنف
            workbook.Save("PlotAreaWidthRatioToChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


