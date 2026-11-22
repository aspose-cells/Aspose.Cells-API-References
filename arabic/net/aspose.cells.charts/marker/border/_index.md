---
title: "Marker.Border"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Marker. تحصل على الحد"
type: docs
url: /ar/net/aspose.cells.charts/marker/border/
---
## Marker.Border property

تحصل على الـ[`border`](../../../aspose.cells.drawing/line/).

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
    public class MarkerPropertyBorderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue(6);

            // إنشاء مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.ScatterConnectedByLinesWithoutDataMarker, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // تكوين السلاسل - إصلاح خطأ التحويل عن طريق الحصول على السلسلة من المجموعة
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A4";
            
            // تخصيص حدود العلامة
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10;
            series.Marker.Area.ForegroundColor = Color.LightBlue;
            series.Marker.Border.FormattingType = ChartLineFormattingType.Solid;
            series.Marker.Border.Color = Color.DarkBlue;
            series.Marker.Border.Weight = WeightType.MediumLine;

            workbook.Save("MarkerBorderDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Line](../../../aspose.cells.drawing/line/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


