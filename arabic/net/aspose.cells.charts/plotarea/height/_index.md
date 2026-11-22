---
title: "PlotArea.Height"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PlotArea. تحصل أو تعين ارتفاع صندوق حدود منطقة الرسم بوحدات 1/4000 من مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/plotarea/height/
---
## PlotArea.Height property

تحصل أو تعين ارتفاع صندوق حدود منطقة الرسم بوحدات 1/4000 من مساحة المخطط.

```csharp
[Obsolete("Use PlotArea.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Height { get; set; }
```

### ملاحظات

مربع حدود مساحة الرسم يشمل مساحة الرسم، علامات الفواصل (تسميات الفواصل)، وإطارًا صغيرًا حول علامات الفواصل. إذا لم يتم إنشاء القيمة بواسطة MS Excel، يرجى استدعاء طريقة Chart.Calculate() قبل استدعاء هذه الطريقة.

الـ **X**, **Y**, **Width** و **Height** لـ **PlotArea** تمثل صندوق الحدود لمنطقة الرسم الذي يشمل منطقة الرسم، علامات الفواصل (تسميات الفواصل)، وحدود صغيرة حول علامات الفواصل. إذا كنت تريد الحصول على الحجم الفعلي لمنطقة الرسم، يجب عليك استدعاء خصائص **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** و **InnerHeightRatioToChart**.

بالنسبة إلى Excel 2007 أو أحدث، القيمة الافتراضية هي صفر. يجب عليك الحصول على القيمة بعد استدعاء Chart.Calculate().

ملاحظة: عند تعيين Height، سيتم تعيين الخاصية IsInnerMode تلقائيًا إلى false.

ملاحظة: هذا العضو أصبح الآن غير صالح. يرجى استخدام خاصية PlotArea.HeightRatioToChart بدلاً من ذلك. Height = HeightRatioToChart * 4000. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyHeightDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // حساب المخطط
            chart.Calculate();

            // عرض خاصية Height
            Console.WriteLine("Chart Area Height: " + chart.ChartArea.Height);
            Console.WriteLine("Plot Area Height: " + chart.PlotArea.Height);

            // تعديل ارتفاع PlotArea
            chart.PlotArea.Height = 2500;
            Console.WriteLine("Modified Plot Area Height: " + chart.PlotArea.Height);
        }
    }
}
```

### انظر أيضًا

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


