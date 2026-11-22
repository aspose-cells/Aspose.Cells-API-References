---
title: "Chart.SecondValueAxis"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية المخطط. تحصل على المحور Y الثاني للمخطط"
type: docs
url: /ar/net/aspose.cells.charts/chart/secondvalueaxis/
---
## Chart.SecondValueAxis property

يحصل على المحور Y الثاني للمخطط.

```csharp
public Axis SecondValueAxis { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySecondValueAxisDemo
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
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(5000);
            worksheet.Cells["C3"].PutValue(3000);
            worksheet.Cells["C4"].PutValue(1000);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // فعّل المحور القيمي الثانوي للسلسلة الثانية
            chart.NSeries[1].PlotOnSecondAxis = true;

            // خصّص المحور القيمي الثانوي
            Axis secondValueAxis = chart.SecondValueAxis;
            secondValueAxis.Title.Text = "Secondary Axis";
            secondValueAxis.MinValue = 0;
            secondValueAxis.MaxValue = 6000;
            secondValueAxis.MajorUnit = 1000;

            // احفظ المصنف
            workbook.Save("SecondValueAxisDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


