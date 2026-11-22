---
title: "الفئة SeriesLayoutProperties"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Charts.SeriesLayoutProperties. تمثل خصائص تخطيط السلسلة"
type: docs
url: /ar/net/aspose.cells.charts/serieslayoutproperties/
---
## SeriesLayoutProperties class

يمثل خصائص تخطيط السلسلة.

```csharp
public class SeriesLayoutProperties
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [SeriesLayoutProperties](serieslayoutproperties/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [IsIntervalLeftClosed](../../aspose.cells.charts/serieslayoutproperties/isintervalleftclosed/) { get; set; } | يشير إلى ما إذا كانت الفاصل مغلقًا من الجانب الأيسر. |
| [MapChartProjectionType](../../aspose.cells.charts/serieslayoutproperties/mapchartprojectiontype/) { get; set; } | يحصل على ويضبط نوع الإسقاط للخريطة. |
| [MapChartRegionType](../../aspose.cells.charts/serieslayoutproperties/mapchartregiontype/) { get; set; } | يحصل على ويضبط نوع المنطقة للخريطة. |
| [MapLabelLayout](../../aspose.cells.charts/serieslayoutproperties/maplabellayout/) { get; set; } | يحصل على ويضبط تخطيط تسميات الخريطة. |
| [QuartileCalculation](../../aspose.cells.charts/serieslayoutproperties/quartilecalculation/) { get; set; } | يمثل الخصائص الإحصائية للسلسلة. |
| [ShowConnectorLines](../../aspose.cells.charts/serieslayoutproperties/showconnectorlines/) { get; set; } | يشير إلى ما إذا كانت خطوط الاتصال معروضة بين نقاط البيانات. |
| [ShowInnerPoints](../../aspose.cells.charts/serieslayoutproperties/showinnerpoints/) { get; set; } | يشير إلى ما إذا كان يجب إظهار نقاط البيانات غير الشاذة. |
| [ShowMeanLine](../../aspose.cells.charts/serieslayoutproperties/showmeanline/) { get; set; } | يشير إلى ما إذا كان يجب إظهار الخط الذي يربط جميع نقاط المتوسط. |
| [ShowMeanMarker](../../aspose.cells.charts/serieslayoutproperties/showmeanmarker/) { get; set; } | يشير إلى ما إذا كانت العلامات التي تدل على المتوسط معروضة. |
| [ShowOutlierPoints](../../aspose.cells.charts/serieslayoutproperties/showoutlierpoints/) { get; set; } | يشير إلى ما إذا كانت نقاط البيانات الشاذة معروضة. |
| [Subtotals](../../aspose.cells.charts/serieslayoutproperties/subtotals/) { get; set; } | يمثل فهرس نقطة بيانات المجموع الفرعي. |

### ملاحظات

ينطبق فقط على مخططات BoxWhisker, Funnel, ParetoLine, Sunburst, Treemap, Waterfall و Histogram.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesLayoutPropertiesDemo
    {
        public static void SeriesLayoutPropertiesExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة سلسلة إلى المخطط
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";
            Series series = chart.NSeries[seriesIndex];

            // تعيين قيم السلسلة
            series.Values = "=B1:B4";

            // الوصول إلى كائن SeriesLayoutProperties
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;

            // تعيين خصائص SeriesLayoutProperties
            layoutProperties.ShowConnectorLines = true;
            layoutProperties.ShowMeanLine = true;
            layoutProperties.ShowOutlierPoints = true;
            layoutProperties.ShowMeanMarker = true;
            layoutProperties.ShowInnerPoints = true;
            layoutProperties.QuartileCalculation = QuartileCalculationType.Inclusive;
            layoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
            layoutProperties.IsIntervalLeftClosed = true;
            layoutProperties.MapChartRegionType = MapChartRegionType.World;
            layoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;

            // احفظ المصنف
            workbook.Save("SeriesLayoutPropertiesExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


