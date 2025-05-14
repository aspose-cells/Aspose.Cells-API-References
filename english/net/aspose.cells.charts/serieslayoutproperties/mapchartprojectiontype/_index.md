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
// Called: chart.NSeries[0].LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;
public static void SeriesLayoutProperties_Property_MapChartProjectionType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet for map chart
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(80);
            worksheet.Cells["B4"].PutValue(60);

            // Add a map chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the chart data range
            chart.SetChartDataRange("A1:B4", true);

            // Set the projection type for the map chart
            chart.NSeries[0].LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;

            // Output the projection type
            Console.WriteLine("Map Chart Projection Type: " + chart.NSeries[0].LayoutProperties.MapChartProjectionType);

            // Save the workbook
            workbook.Save("MapChartProjectionTypeExample.xlsx");
        }
```

### See Also

* enum [MapChartProjectionType](../../mapchartprojectiontype/)
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


