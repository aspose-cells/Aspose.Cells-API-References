---
title: "ChartFrame.HeightRatioToChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تحصل أو تعين ارتفاع الإطار بوحدات نسبة مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/heightratiotochart/
---
## ChartFrame.HeightRatioToChart property

يحصل على أو يضبط ارتفاع الإطار بوحدات نسبة مساحة المخطط.

```csharp
public virtual double HeightRatioToChart { get; set; }
```

### ملاحظات

هذه قيمة كسرية، نطاقها الصحيح بين 0-1. كيف يتم تحويل وحدات النسبة إلى بكسل؟ HeightPixel = HeightRatioToChart * Chart.ChartObject.Height;

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightRatioToChartDemo
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
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى عنوان المخطط (الذي يرث من ChartFrame)
            chart.Title.Text = "Sample Chart";
            ChartFrame titleFrame = chart.Title;

            // عرض قيمة HeightRatioToChart الحالية
            Console.WriteLine("Current HeightRatioToChart value: " + titleFrame.HeightRatioToChart);

            // اضبط نسبة ارتفاع جديدة (0.1 = 10% من ارتفاع المخطط)
            titleFrame.HeightRatioToChart = 0.1;

            // إظهار التأثير بالمقارنة بين قبل/بعد
            Console.WriteLine("Title height reduced to 10% of chart height");

            // حفظ النتيجة
            workbook.Save("PropertyHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


