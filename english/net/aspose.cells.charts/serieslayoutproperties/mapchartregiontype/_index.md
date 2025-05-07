---
title: SeriesLayoutProperties.MapChartRegionType
second_title: Aspose.Cells for .NET API Reference
description: SeriesLayoutProperties property. Gets and sets the region type of the map
type: docs
url: /net/aspose.cells.charts/serieslayoutproperties/mapchartregiontype/
---
## SeriesLayoutProperties.MapChartRegionType property

Gets and sets the region type of the map.

```csharp
public MapChartRegionType MapChartRegionType { get; set; }
```

### Examples

```csharp
// Called: layoutProperties.MapChartRegionType = MapChartRegionType.World;
public static void Property_MapChartRegionType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
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

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add series to the chart
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";
            Series series = chart.NSeries[seriesIndex];

            // Set the values of the series
            series.Values = "=B1:B4";

            // Access the SeriesLayoutProperties object
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;

            // Set properties of SeriesLayoutProperties
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

            // Save the workbook
            workbook.Save("SeriesLayoutPropertiesExample.xlsx");
        }
```

### See Also

* enum [MapChartRegionType](../../mapchartregiontype/)
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


