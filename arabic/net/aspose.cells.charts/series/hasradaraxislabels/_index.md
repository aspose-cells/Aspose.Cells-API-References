---
title: "Series.HasRadarAxisLabels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. صحيحة إذا كان مخطط الرادار يحتوي على تسميات محور الفئة. ينطبق فقط على مخططات الرادار"
type: docs
url: /ar/net/aspose.cells.charts/series/hasradaraxislabels/
---
## Series.HasRadarAxisLabels property

صحيح إذا كان مخطط الرادار يحتوي على تسميات محور الفئة. ينطبق فقط على مخططات الرادار.

```csharp
public bool HasRadarAxisLabels { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasRadarAxisLabelsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة لمخطط الرادار
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(2);
            worksheet.Cells["B4"].PutValue(5);

            // أضف مخطط رادار
            int chartIndex = worksheet.Charts.Add(ChartType.Radar, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة بيانات السلسلة
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على السلسلة واضبط تسميات محور الرادار
            Series series = chart.NSeries[seriesIndex];
            series.HasRadarAxisLabels = true; // This is the key property being demonstrated

            // احفظ المصنف
            workbook.Save("RadarChartWithAxisLabels.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


