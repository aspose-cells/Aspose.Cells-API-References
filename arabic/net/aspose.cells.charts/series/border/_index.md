---
title: "Series.Border"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. تمثل حدود كائن Series"
type: docs
url: /ar/net/aspose.cells.charts/series/border/
---
## Series.Border property

يمثل حد كائن Series.

```csharp
public Line Border { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBorderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["A2"].PutValue("2020");
            worksheet.Cells["A3"].PutValue("2021");
            worksheet.Cells["A4"].PutValue("2022");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(5000);
            worksheet.Cells["B3"].PutValue(7000);
            worksheet.Cells["B4"].PutValue(9000);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة بيانات السلسلة
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على السلسلة الأولى
            Series series = chart.NSeries[0];
            series.Name = "Sales Data";

            // خصص خصائص الحدود
            series.Border.Color = System.Drawing.Color.Blue;
            series.Border.Weight = WeightType.MediumLine;
            series.Border.DashType = MsoLineDashStyle.Solid;
            series.Border.IsVisible = true;

            // احفظ المصنف
            workbook.Save("SeriesBorderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


