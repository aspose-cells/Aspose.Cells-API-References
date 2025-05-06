---
title: SeriesLayoutProperties.MapChartProjectionType
second_title: Aspose.Cells for .NET API Reference
description: SeriesLayoutProperties property. Gets and sets the projection type of the map
type: docs
url: /net/aspose.cells.charts/serieslayoutproperties/mapchartprojectiontype/
---
## SeriesLayoutProperties.MapChartProjectionType property

Gets and sets the projection type of the map.

```csharp
public MapChartProjectionType MapChartProjectionType { get; set; }
```

### Examples

```csharp
// Called: layoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;
public static void Property_MapChartProjectionType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(50);
            worksheet.Cells[&quot;A2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(150);
            worksheet.Cells[&quot;A4&quot;].PutValue(200);
            worksheet.Cells[&quot;B1&quot;].PutValue(60);
            worksheet.Cells[&quot;B2&quot;].PutValue(32);
            worksheet.Cells[&quot;B3&quot;].PutValue(50);
            worksheet.Cells[&quot;B4&quot;].PutValue(40);
            worksheet.Cells[&quot;C1&quot;].PutValue(&quot;Q1&quot;);
            worksheet.Cells[&quot;C2&quot;].PutValue(&quot;Q2&quot;);
            worksheet.Cells[&quot;C3&quot;].PutValue(&quot;Y1&quot;);
            worksheet.Cells[&quot;C4&quot;].PutValue(&quot;Y2&quot;);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add series to the chart
            int seriesIndex = chart.NSeries.Add(&quot;A1:B4&quot;, true);
            chart.NSeries.CategoryData = &quot;C1:C4&quot;;
            Series series = chart.NSeries[seriesIndex];

            // Set the values of the series
            series.Values = &quot;=B1:B4&quot;;

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
            workbook.Save(&quot;SeriesLayoutPropertiesExample.xlsx&quot;);
        }
```

### See Also

* enum [MapChartProjectionType](../../mapchartprojectiontype/)
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


