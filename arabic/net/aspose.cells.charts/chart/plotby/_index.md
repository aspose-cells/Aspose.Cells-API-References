---
title: "Chart.PlotBy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. تحصل وتضبط ما إذا كان الرسم حسب الصف أو العمود"
type: docs
url: /ar/net/aspose.cells.charts/chart/plotby/
---
## Chart.PlotBy property

يحصل ويعيّن ما إذا كان الرسم حسب الصف أو العمود.

```csharp
public PlotDataByType PlotBy { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotByDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.SetChartDataRange("A1:C4", true);

            // عرض خاصية PlotBy
            Console.WriteLine("Default PlotBy: " + chart.PlotBy);
            
            // إنشاء مخطط جديد مع إعداد plot مختلف
            int newChartIndex = worksheet.Charts.Add(ChartType.Column, 25, 0, 40, 8);
            Aspose.Cells.Charts.Chart newChart = worksheet.Charts[newChartIndex];
            newChart.SetChartDataRange("A1:C4", false); // Plot by row
            Console.WriteLine("New chart PlotBy: " + newChart.PlotBy);

            // احفظ المصنف
            workbook.Save("ChartPropertyPlotByDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PlotDataByType](../../plotdatabytype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


