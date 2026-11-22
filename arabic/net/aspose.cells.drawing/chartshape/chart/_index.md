---
title: "ChartShape.Chart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartShape. تُرجع كائن Chart يمثل المخطط الموجود داخل الكائن"
type: docs
url: /ar/net/aspose.cells.drawing/chartshape/chart/
---
## ChartShape.Chart property

يرجع كائن Chart الذي يمثل المخطط الموجود داخل الكائن.

```csharp
public Chart Chart { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ChartShapePropertyChartDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Grains");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على نسخة ChartShape
            ChartShape chartShape = (ChartShape)chart.ChartObject;

            // الوصول إلى خاصية Chart (للقراءة فقط)
            Chart accessedChart = chartShape.Chart;

            // عرض خصائص المخطط
            Console.WriteLine("Chart Name: " + accessedChart.Name);
            Console.WriteLine("Chart Type: " + accessedChart.Type);
            Console.WriteLine("Show Legend: " + accessedChart.ShowLegend);

            // تعديل خصائص المخطط عبر كائن Chart
            accessedChart.Name = "Sales Chart";
            accessedChart.ShowLegend = false;
            accessedChart.Title.Text = "Product Sales Distribution";

            // تغيير نوع المخطط
            accessedChart.Type = ChartType.Pie;

            // حفظ النتيجة
            workbook.Save("ChartShapePropertyChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../../../aspose.cells.charts/chart/)
* class [ChartShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


