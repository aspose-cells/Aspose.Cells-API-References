---
title: "SeriesLayoutProperties.ShowMeanMarker"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SeriesLayoutProperties. تشير إلى ما إذا كانت العلامات التي تمثل المتوسط معروضة"
type: docs
url: /ar/net/aspose.cells.charts/serieslayoutproperties/showmeanmarker/
---
## SeriesLayoutProperties.ShowMeanMarker property

يشير إلى ما إذا كانت العلامات التي تدل على المتوسط معروضة.

```csharp
public bool ShowMeanMarker { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowMeanMarkerDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // إنشاء مخطط (باستخدام نوع مخطط العمود الذي يدعم علامات المتوسط)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة
            chart.NSeries.Add("A1:A4", true);
            Series series = chart.NSeries[0];

            // تكوين خصائص التخطيط باستخدام ShowMeanMarker
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;
            layoutProperties.ShowMeanMarker = true;
            layoutProperties.ShowMeanLine = true;

            // احفظ الناتج
            workbook.Save("ColumnChartWithMeanMarker.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


