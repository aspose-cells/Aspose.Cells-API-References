---
title: "PlotArea.XRatioToChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PlotArea. تحصّل أو تعين إحداثي x للزاوية العلوية اليسرى لصندوق حدود منطقة الرسم كنسبة من مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/plotarea/xratiotochart/
---
## PlotArea.XRatioToChart property

يحصل أو يحدد إحداثي x للزاوية العليا اليسرى لصندوق حدود مساحة الرسم كنسبة من مساحة المخطط.

```csharp
public override double XRatioToChart { get; set; }
```

### ملاحظات

مربع حدود مساحة الرسم يشمل مساحة الرسم، علامات الفواصل (تسميات الفواصل)، وإطارًا صغيرًا حول علامات الفواصل. إذا لم يتم إنشاء القيمة بواسطة MS Excel، يرجى استدعاء طريقة Chart.Calculate() قبل استدعاء هذه الطريقة.

الـ **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** و **HeightRatioToChart** لـ **PlotArea** تمثل صندوق الحدود لمنطقة الرسم الذي يشمل منطقة الرسم، علامات الفواصل (تسميات الفواصل)، وحدود صغيرة حول علامات الفواصل. إذا كنت تريد الحصول على الحجم الفعلي لمنطقة الرسم، يجب عليك استدعاء خصائص **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** و **InnerHeightRatioToChart**.

بالنسبة إلى Excel 2007 أو أحدث، القيمة الافتراضية هي صفر. يجب عليك الحصول على القيمة بعد استدعاء Chart.Calculate().

XPixel = XRatioToChart * chart.ChartObject.Width. ملاحظة: عندما يتم تعيين XRatioToChart، سيتم تعيين خاصية IsInnerMode تلقائيًا إلى false.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyXRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // احصل على منطقة الرسم للمخطط
            PlotArea plotArea = chart.PlotArea;

            // عرض القيمة الحالية لـ XRatioToChart
            Console.WriteLine("Current XRatioToChart value: " + plotArea.XRatioToChart);

            // غيّر قيمة XRatioToChart لتحريك منطقة الرسم أفقيًا
            plotArea.XRatioToChart = 0.2; // 20% from the left of the chart area

            // عرض القيمة الجديدة لـ XRatioToChart
            Console.WriteLine("New XRatioToChart value: " + plotArea.XRatioToChart);

            // حفظ المصنف لرؤية التأثير
            workbook.Save("PlotAreaXRatioToChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


