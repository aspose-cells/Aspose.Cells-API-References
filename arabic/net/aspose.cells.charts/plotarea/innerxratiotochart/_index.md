---
title: "PlotArea.InnerXRatioToChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PlotArea. تحصل أو تسترجع إحداثي x للزاوية العلوية العليا لمنطقة الرسم بوحدات نسبة مساحة المخطط."
type: docs
url: /ar/net/aspose.cells.charts/plotarea/innerxratiotochart/
---
## PlotArea.InnerXRatioToChart property

يحصل أو يحصل على إحداثي x للزاوية العليا العليا لمساحة الرسم بوحدات نسبة مساحة المخطط.

```csharp
public double InnerXRatioToChart { get; set; }
```

### ملاحظات

مربع حدود مساحة الرسم يشمل مساحة الرسم، علامات الفواصل (تسميات الفواصل)، وإطارًا صغيرًا حول علامات الفواصل. إذا لم يتم إنشاء القيمة بواسطة MS Excel، يرجى استدعاء طريقة Chart.Calculate() قبل استدعاء هذه الطريقة.

الـ **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** و **HeightRatioToChart** لـ **PlotArea** تمثل صندوق الحدود لمنطقة الرسم الذي يشمل منطقة الرسم، علامات الفواصل (تسميات الفواصل)، وحدود صغيرة حول علامات الفواصل. إذا كنت تريد الحصول على الحجم الفعلي لمنطقة الرسم، يجب عليك استدعاء خصائص **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** و **InnerHeightRatioToChart**.

بالنسبة إلى Excel 2007 أو أحدث، القيمة الافتراضية هي صفر. يجب عليك الحصول على القيمة بعد استدعاء Chart.Calculate().

InnerX بالبكسل = InnerXRatioToChart * chart.ChartObject.Width. ملاحظة: عندما يتم تعيين InnerXRatioToChart، سيتم ضبط خاصية IsInnerMode تلقائيًا إلى True.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyInnerXRatioToChartDemo
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

            // اعرض القيمة الحالية لـ InnerXRatioToChart
            Console.WriteLine("Current InnerXRatioToChart value: " + plotArea.InnerXRatioToChart);

            // حدد قيمة جديدة لـ InnerXRatioToChart (تحريك منطقة الرسم إلى اليمين)
            plotArea.InnerXRatioToChart = 0.2;

            // اعرض القيمة الجديدة
            Console.WriteLine("New InnerXRatioToChart value: " + plotArea.InnerXRatioToChart);

            // حفظ المصنف لرؤية التأثير
            workbook.Save("PlotAreaPropertyInnerXRatioToChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


