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
// Called: series.LayoutProperties.MapChartRegionType = MapChartRegionType.CountryRegionList;
public static void Property_MapChartRegionType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Country&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;USA&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Canada&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;Mexico&quot;);

            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Value&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(100);
            worksheet.Cells[&quot;B3&quot;].PutValue(200);
            worksheet.Cells[&quot;B4&quot;].PutValue(300);

            // Add a map chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the chart data range
            chart.SetChartDataRange(&quot;A1:B4&quot;, true);

            // Set the region type of the map chart
            foreach (Series series in chart.NSeries)
            {
                series.LayoutProperties.MapChartRegionType = MapChartRegionType.CountryRegionList;
            }

            // Save the workbook
            workbook.Save(&quot;MapChartRegionTypeExample.xlsx&quot;);

            // Output the result
            Console.WriteLine(&quot;Map chart with region type &apos;CountryRegionList&apos; created successfully.&quot;);
        }
```

### See Also

* enum [MapChartRegionType](../../mapchartregiontype/)
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


