---
title: "Chart.SeriesAxis"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. تحصل على محور السلسلة للمخطط"
type: docs
url: /ar/net/aspose.cells.charts/chart/seriesaxis/
---
## Chart.SeriesAxis property

يحصل على محور السلسلة للمخطط.

```csharp
public Axis SeriesAxis { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySeriesAxisDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Product B");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // إضافة مخطط عمودي مجمع ثلاثي الأبعاد
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B1:C4", true);

            // الوصول إلى SeriesAxis وتكوينه
            Axis seriesAxis = chart.SeriesAxis;
            seriesAxis.Title.Text = "Product Series";
            seriesAxis.Title.Font.Size = 12;
            seriesAxis.Title.Font.IsBold = true;
            seriesAxis.MajorTickMark = TickMarkType.Cross;
            seriesAxis.MinorTickMark = TickMarkType.Outside;

            // احفظ المصنف
            workbook.Save("ChartPropertySeriesAxisDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


