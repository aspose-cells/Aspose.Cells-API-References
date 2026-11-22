---
title: "ChartFrame.YRatioToChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تحصل أو تعين إحداثي y للزاوية العليا اليسرى بوحدات نسبة مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/yratiotochart/
---
## ChartFrame.YRatioToChart property

يحصل على أو يضبط إحداثي y للزاوية العليا اليسرى بوحدات نسبة مساحة المخطط.

```csharp
public virtual double YRatioToChart { get; set; }
```

### ملاحظات

هذه قيمة كسرية، نطاقها الصالح بين 0-1. كيف يمكن تحويل وحدات النسبة إلى بكسلات؟ YPixel = YRatioToChart * Chart.ChartObject.Height;

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyYRatioToChartDemo
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
            
            // الوصول إلى عنوان المخطط الذي يرث من ChartFrame
            chart.Title.Text = "Sample Chart";
            
            // عرض قيمة YRatioToChart الحالية
            Console.WriteLine("Current Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // غيّر موضع Y للعنوان بالنسبة إلى مساحة المخطط
            chart.Title.YRatioToChart = 0.1; // 10% from top of chart area
            
            // عرض قيمة YRatioToChart الجديدة
            Console.WriteLine("New Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // الوصول إلى legend الذي يرث أيضًا من ChartFrame
            chart.Legend.Position = LegendPositionType.Top;
            
            // عرض قيمة YRatioToChart الحالية للـ legend
            Console.WriteLine("Current Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // غيّر موضع Y للـ legend بالنسبة إلى مساحة المخطط
            chart.Legend.YRatioToChart = 0.15; // 15% from top of chart area
            
            // عرض قيمة YRatioToChart الجديدة للـ legend
            Console.WriteLine("New Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // احفظ المصنف
            workbook.Save("ChartFramePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


