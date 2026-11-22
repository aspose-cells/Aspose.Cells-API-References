---
title: "SeriesLayoutProperties.MapLabelLayout"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SeriesLayoutProperties. تحصل وتعيّن تخطيط تسميات الخريطة"
type: docs
url: /ar/net/aspose.cells.charts/serieslayoutproperties/maplabellayout/
---
## SeriesLayoutProperties.MapLabelLayout property

يحصل على ويضبط تخطيط تسميات الخريطة.

```csharp
public MapChartLabelLayout MapLabelLayout { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyMapLabelLayoutDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة لمخطط الخريطة
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("United States");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["B3"].PutValue(80);
            worksheet.Cells["A4"].PutValue("Mexico");
            worksheet.Cells["B4"].PutValue(60);

            // أضف مخطط خريطة
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            Series series = chart.NSeries[0];
            series.XValues = "A2:A4";

            // تكوين خصائص تخطيط الخريطة
            series.LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;
            series.LayoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
            series.LayoutProperties.MapChartRegionType = MapChartRegionType.DataOnly;

            // احفظ المصنف
            workbook.Save("MapLabelLayoutDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [MapChartLabelLayout](../../mapchartlabellayout/)
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


