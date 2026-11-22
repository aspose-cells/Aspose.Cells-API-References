---
title: "PlotArea.HeightRatioToChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PlotArea. تحصّل أو تعين ارتفاع صندوق حدود منطقة الرسم بوحدات نسبة مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/plotarea/heightratiotochart/
---
## PlotArea.HeightRatioToChart property

يحصل أو يحدد ارتفاع صندوق حدود مساحة الرسم بوحدات نسبة مساحة المخطط.

```csharp
public override double HeightRatioToChart { get; set; }
```

### ملاحظات

مربع حدود مساحة الرسم يشمل مساحة الرسم، علامات الفواصل (تسميات الفواصل)، وإطارًا صغيرًا حول علامات الفواصل. إذا لم يتم إنشاء القيمة بواسطة MS Excel، يرجى استدعاء طريقة Chart.Calculate() قبل استدعاء هذه الطريقة.

الـ **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** و **HeightRatioToChart** لـ **PlotArea** تمثل صندوق الحدود لمنطقة الرسم الذي يشمل منطقة الرسم، علامات الفواصل (تسميات الفواصل)، وحدود صغيرة حول علامات الفواصل. إذا كنت تريد الحصول على الحجم الفعلي لمنطقة الرسم، يجب عليك استدعاء خصائص **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** و **InnerHeightRatioToChart**.

بالنسبة إلى Excel 2007 أو أحدث، القيمة الافتراضية هي صفر. يجب عليك الحصول على القيمة بعد استدعاء Chart.Calculate().

HeightPixel = HeightRatioToChart * chart.ChartObject.Width. ملاحظة: عندما يتم تعيين HeightRatioToChart، سيتم تعيين خاصية IsInnerMode تلقائيًا إلى false.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyHeightRatioToChartDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على منطقة الرسم للمخطط
            PlotArea plotArea = chart.PlotArea;

            // عرض نسبة الارتفاع الحالية
            Console.WriteLine("Current HeightRatioToChart value: " + plotArea.HeightRatioToChart);

            // تعيين نسبة ارتفاع جديدة (0.7 تعني 70٪ من ارتفاع مساحة المخطط)
            plotArea.HeightRatioToChart = 0.7;

            // عرض نسبة الارتفاع الجديدة
            Console.WriteLine("New HeightRatioToChart value: " + plotArea.HeightRatioToChart);

            // حفظ المصنف لرؤية التأثير
            workbook.Save("PlotAreaHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


